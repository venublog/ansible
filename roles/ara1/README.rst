ansible-role-ara
================

Ansible role to install and configure ARA on Fedora, RHEL, Fedora as well as
Debian and Ubuntu.


Using the role
--------------

The default parameters of the role will install ARA and configure a persistent
systemd service to run the embedded development server::

    mkdir roles
    git clone https://git.openstack.org/openstack/ansible-role-ara roles/ara
    cat << EOF > playbook.yml
    - name: Install ARA with default settings
      hosts: localhost
      roles:
        - ara
    EOF
    ansible-playbook playbook.yml

    (at your option) any later version.

    ARA is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with ARA.  If not, see <http://www.gnu.org/licenses/>.
