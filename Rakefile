=begin
Version: MPL 1.1/GPL 2.0/LGPL 2.1

"The contents of this file are subject to the Mozilla Public License Version
1.1 (the "License"); you may not use this file except in compliance with the
License. You may obtain a copy of the License at http://www.mozilla.org/MPL/

Software distributed under the License is distributed on an "AS IS" basis,
WITHOUT WARRANTY OF ANY KIND, either express or implied. See the License for
the specific language governing rights and limitations under the License.

The Original Code is pdf_license, released June 5th, 2010. The Initial
Developer of the Original Code is consiliens (consiliens@gmail.com). Portions
created by consiliens are Copyright (C) 2010 consiliens
(consiliens@gmail.com). All Rights Reserved.

Alternatively, the contents of this file may be used under the terms of the
GNU Lesser General Public License Version 2.1 or later (the "LGPL" License),
in which case the provisions of the LGPL License are applicable instead of
those above. If you wish to allow use of your version of this file only under
the terms of the LGPL License and not to allow others to use your version of
this file under the MPL, indicate your decision by deleting the provisions
above and replace them with the notice and other provisions required by the
LGPL License. If you do not delete the provisions above, a recipient may use
your version of this file under either the MPL or the LGPL License."
=end
# encoding: UTF-8

$:.unshift 'lib'

require 'rubygems'
require 'rspec/core/rake_task'

task :default => :spec

desc 'Run RSpec specs'
RSpec::Core::RakeTask.new :spec do | task |
  task.pattern = FileList['spec/**/*_spec.rb']
end

desc 'Run main.rb'
task :main do
  require 'main'
  Main.run
end
