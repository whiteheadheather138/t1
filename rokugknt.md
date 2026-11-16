代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qzl.fanxiaobao.xyz

[R08] 数值比较
来源：http://gxz.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://noz.cashguo.top

[R09] 字符串比较
来源：http://cys.bjfxy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://opr.9152youxi.cn

[R10] 正则匹配
来源：http://cnc.jinqigfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vdi.yj202588.top

[R11] case 多分支
来源：http://dea.hammf.cn

case "$1" in
来源：http://zmp.xuanzx.com

start) echo "启动" ;;
来源：http://szb.hysaishi.cn

stop)  echo "停止" ;;
来源：http://zaw.zhixingplan.top

*)     echo "未知命令" ;;
来源：http://ovw.ppjwa.cn

esac
来源：http://kjb.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://gyc.fehbvm.com

for f in *.txt; do echo "$f"; done
来源：http://alh.pycfn.com

[R13] for 计数循环
来源：http://exb.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://tmx.ywan-chungtsiang.top

[R14] C 风格 for
来源：http://isx.zycfv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pcx.hcnkem.com

[R15] while 逐行读文件
来源：http://uop.daria6918.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://emd.316326.xyz

[R16] until 等待条件
来源：http://mzl.daxiang520.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nnr.ywan-chungtsiang.top

[R17] 数组定义与取值
来源：http://rct.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://svx.fzhhl.top

[R18] 遍历数组
来源：http://kmb.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yzq.jinghuilouyu.cn

[R19] 数组长度
来源：http://paj.daxiang520.top

echo "${#arr[@]}"
来源：http://kfs.fanxiaobao.xyz

[R20] 关联数组（字典）
来源：http://awc.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nlt.jinqigfzy.top

[R21] 字符串长度
来源：http://ukk.yonumen.top

echo "${#s}"
来源：http://ldh.nwbrower.top

[R22] 截取子串
来源：http://dyx.xziqi.cn

echo "${s:0:5}"
来源：http://hda.kuanghao11.cn

[R23] 字符串替换
来源：http://udl.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qcl.hysaishi.cn

[R24] 大小写转换
来源：http://tso.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zqq.cqqwz.cn

[R25] 去后缀 / 去前缀
来源：http://vtx.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fws.chenzaomai.com

[R26] 命令替换
来源：http://mgv.jinyuanbaomall.cn

now=$(date +%F); echo "$now"
来源：http://xjo.dashuyun.cn

[R27] 算术展开
来源：http://wgb.zhengqikj.top

echo $((1 + 2 * 3))
来源：http://lai.ehwqpu.com

[R28] 浮点运算
来源：http://qze.shanyushiyangtech.top

echo "scale=2; 10/3" | bc
来源：http://eex.sxryk.cn

[R29] 定义函数
来源：http://qyz.zhiwuduotai.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oea.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://rkc.andypj.xyz

f() { return 0; }; f || echo "失败了"
来源：http://lmc.sjlbkw.cn

[R31] 局部变量
来源：http://pyv.cucudq.cn

f() { local x=1; echo "$x"; }
来源：http://ucq.iojbl.cn

[R32] 参数个数校验
来源：http://aea.jlsjyb.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cla.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://rtj.shangyingyoupin.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tko.nanxuanxn.top

[R34] 退出时清理
来源：http://imv.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ain.hammf.cn

[R35] 后台执行并等待
来源：http://xhj.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lce.kuanghao11.cn

[R36] 并发执行多个任务
来源：http://udv.wangdashe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://exy.fehbvm.com

[R37] 把输出赋给变量
来源：http://kpa.9152youxi.cn

files=$(ls -1)
来源：http://ubi.yanxiufei.cn

[R38] 管道串联
来源：http://pvz.nanxinkj.top

cat a.txt | grep -i error | wc -l
来源：http://aug.sweek.top

[R39] 重定向标准输出与错误
来源：http://ugj.yvedp.cn

cmd > out.log 2>&1
来源：http://ght.aibaodan.cn

[R40] 追加写日志
来源：http://cgu.yangfankeji.com

echo "log" >> out.log
来源：http://zci.xuanzx.com

[R41] 丢弃输出
来源：http://zhx.tian-w.cn

cmd >/dev/null 2>&1
来源：http://hex.chenzaomai.com

[R42] 输入重定向
来源：http://qbo.gotoacloud.top

wc -l < a.txt
来源：http://tfs.yuanzhike.top

[R43] 按名字查找文件
来源：http://vkw.shangyingyoupin.top

find . -name "*.log" -type f
来源：http://dar.ctjpmb.com

[R44] 按修改时间查找
来源：http://ttr.bjfxy.top

find . -mtime -7 -type f
来源：http://sab.ydzc1.top

[R45] 批量删除
来源：http://obd.meibo888.top

find . -name "*.tmp" -delete
来源：http://tqx.havefunace.top

[R46] 递归替换文件内容
来源：http://qli.bbcook.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hzp.birdmap.top

[R47] sed 单行替换
来源：http://uje.yfazqb.com

sed -i 's/foo/bar/g' a.txt
来源：http://rti.yueranfly.top

[R48] awk 取指定列
来源：http://ppg.jyoumei.cn

awk '{print $1, $3}' a.txt
来源：http://xan.hnxiangtu.top

[R49] awk 带条件
来源：http://fub.andypj.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pqp.sufxvd.cn

[R50] awk 求和
来源：http://rto.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dph.pycfn.com

[R51] 排序去重取前几
来源：http://svt.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mze.jinqigufen.top

[R52] 统计行数
来源：http://tum.shuidangran.top

wc -l a.txt
来源：http://gva.chenzaomai.com

[R53] 查看文件头与实时尾
来源：http://rah.havefunace.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dhm.cqqwz.cn

[R54] 比较两个文件
来源：http://ksk.yvedp.cn

diff a.txt b.txt
来源：http://vhh.yvedp.cn

[R55] 压缩与解压
来源：http://ujn.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ftd.zdbjq.cn

[R56] 远程拷贝
来源：http://znw.sxryk.cn

scp file user@host:/path/
来源：http://fdr.fktsv.cn

[R57] 远程执行命令
来源：http://vue.sxryk.cn

ssh user@host 'uptime'
来源：http://bpk.yangfankeji.com

[R58] 下载文件
来源：http://bqf.yongpay.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://msg.sjlbkw.cn

[R59] 发 POST JSON
来源：http://yxq.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oic.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://epk.jinqigufen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oba.yj202588.top

[R61] 磁盘占用
来源：http://ajp.hywenlv.cn

df -h;  du -sh *
来源：http://qig.feifeiyinyue.top

[R62] 找最占空间的文件
来源：http://cei.hammf.cn

du -ah . | sort -rh | head -10
来源：http://gyu.xingfuxueyuan.xyz

[R63] 内存与进程
来源：http://grs.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://hoi.vehdjk.com

[R64] 结束进程
来源：http://evz.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://alm.dianchejie.cn

[R65] 查看端口占用
来源：http://gge.xingfuxueyuan.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://omg.fanxiaobao.xyz

[R66] 定时任务
来源：http://crz.dianchejie.cn

crontab -e;  crontab -l
来源：http://ctw.jianghu66.top

[R67] 生成随机十六进制串
来源：http://wnx.fengsongda.top

openssl rand -hex 16
来源：http://ofe.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://bkn.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://bdo.tanke756.top

[R69] 生成随机密码
来源：http://xuo.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://wgp.hysaishi.cn

[R70] 时间戳与互转
来源：http://vwv.dashuyun.cn

date +%s;  date -d @1700000000
来源：http://pux.yonumen.top

[R71] 日期格式化
来源：http://zxp.shangyingyoupin.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fmv.shuidangran.top

[R72] 等待端口就绪
来源：http://ani.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xpy.chenjidiqi.icu

[R73] 分割大日志
来源：http://wrb.hysaishi.cn

split -l 1000 big.log part_
来源：http://wth.hnxiangtu.top

[R74] 批量重命名
来源：http://mkv.nanxinkj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qef.hammf.cn

[R75] 导出环境变量
来源：http://fbv.snrcjt.cn

export PATH="$HOME/bin:$PATH"
来源：http://zna.pengpengdd.cyou

[R76] 使用临时文件
来源：http://lql.ybcxt.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bwo.tianlin.xyz

[R77] 读取用户输入
来源：http://ghe.mhx1999.top

read -rp "请输入: " ans
来源：http://epp.quarkkingdee.top

[R78] 交互式菜单
来源：http://afp.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rjh.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://tzm.yanxiufei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vlh.pycfn.com

[R80] 查看脚本执行耗时
来源：http://ang.yvedp.cn

time ./run.sh
来源：http://lac.sxryk.cn

================================================================================
来源：http://fdg.gogol.net.cn

S. C / C++ 专题
来源：http://tbn.0kj1m.cn

================================================================================
来源：http://wvz.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://adt.haohaochexian.top

#include <stdio.h>
来源：http://jzj.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bpv.havefunace.top

[S02] C：变量与格式化输出
来源：http://yza.zycfv.cn

int a = 10; printf("%d\n", a);
来源：http://yhn.tian-w.cn

[S03] C：读入整数
来源：http://dup.tian-w.cn

int x; scanf("%d", &x);
来源：http://kdr.jiagoushi.top

[S04] C：字符串复制
来源：http://itg.zdqjudy.top

char dst[32]; strcpy(dst, "hi");
来源：http://udp.nwbrower.top

[S05] C：字符串长度
来源：http://jme.yueranfly.top

strlen(s)
来源：http://urp.sufxvd.cn

[S06] C：字符串比较
来源：http://cra.zdqjudy.top

strcmp(a, b) == 0
来源：http://ajy.cheryme.top

[S07] C：数组遍历求和
来源：http://wpk.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cwu.yvedp.cn

[S08] C：动态内存分配与释放
来源：http://xul.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hrw.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://bzm.hnqzz.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bfw.kuanghao11.cn

[S10] C：指针与解引用
来源：http://hhc.yangfankeji.com

int *p = &a;  *p = 5;
来源：http://otf.yongpay.top

[S11] C：逐行读文件
来源：http://tdw.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://lyw.hesvh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zej.andypj.xyz

fclose(f);
来源：http://lgl.zhaomingkeji.xyz

[S12] C：写文件
来源：http://dag.zdbjq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eul.ppjwa.cn

[S13] C：宏定义
来源：http://twk.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://arp.zhijiandao.cn

[S14] C：枚举
来源：http://ldg.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://guz.vehdjk.com

[S15] C：类型转换
来源：http://fcy.yongpay.top

(double) a / b
来源：http://rbw.snrcjt.cn

[S16] C：位操作置位
来源：http://uzm.redwolf501.top

x |= (1 << 3);
来源：http://acf.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://hmh.iojbl.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wbm.hcnkem.com

[S18] C：命令行参数
来源：http://xjo.sweek.top

int main(int argc, char **argv)
来源：http://evw.jqgfzy.top

[S19] C：快速排序
来源：http://ukl.shanyushiyangtech.top

qsort(a, n, sizeof(int), cmp);
来源：http://rrr.316326.xyz

[S20] C：二分查找
来源：http://qnq.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cbm.gzhubu.top

[S21] C：字符类别判断
来源：http://jsl.cucudq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xju.tian-w.cn

[S22] C：字符串转数字
来源：http://ape.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ckx.shangyingyoupin.top

[S23] C：随机数
来源：http://auk.zhaomingkeji.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://qwm.yongpay.top

[S24] C：获取本地时间
来源：http://fnv.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://izq.jqgufenzy.top

[S25] C：内存拷贝
来源：http://epi.fengsongda.top

memcpy(dst, src, n);
来源：http://bhc.svipenyu.cn

[S26] C：内存清零
来源：http://bzd.sweek.top

memset(a, 0, sizeof a);
来源：http://vva.jiagoushi.top

[S27] C：定义常量
来源：http://jxl.vehdjk.com

const double PI = 3.14159;
来源：http://aph.fehbvm.com

[S28] C：静态变量
来源：http://znd.fanxiaobao.xyz

static int counter = 0;
来源：http://ejl.cashguo.top

[S29] C：变参函数
来源：http://bwh.nanxuanxn.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qim.yanxiufei.cn

[S30] C：头文件保护
来源：http://ngj.jlsjyb.cn

#ifndef X_H
来源：http://dfy.nwbrower.top

#define X_H
来源：http://mni.zhiwuduotai.top

#endif
来源：http://iyi.yongpay.top

[S31] C++：Hello World
来源：http://vmi.guannengcc.top

#include <iostream>
来源：http://vcz.hongshengwenyu.top

int main() { std::cout << "Hello\n"; }
来源：http://gtd.xinyue.icu

[S32] C++：字符串
来源：http://mck.tanke756.top

std::string s = "hi";  s += "!";
来源：http://fzg.gzhubu.top

[S33] C++：vector 增删
来源：http://cde.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ncc.0kj1m.cn

[S34] C++：遍历 vector
来源：http://uhu.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://iyx.shzxlz.cn

[S35] C++：map
来源：http://xwg.sjlbkw.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xqo.bjfxy.top

[S36] C++：unordered_map
来源：http://euu.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vbm.jinyuanbaomall.cn

[S37] C++：set
来源：http://dai.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cjo.jianghu66.top

[S38] C++：排序
来源：http://wwo.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://nyg.zycfv.cn

[S39] C++：自定义比较器排序
来源：http://qwv.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://plj.xuetiantiany.cn

[S40] C++：查找元素
来源：http://qve.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tjx.jlsjyb.cn

[S41] C++：类与构造函数
来源：http://svi.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pvz.0kj1m.cn

[S42] C++：继承与虚函数
来源：http://rbc.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://jzq.cashguo.top

[S43] C++：智能指针
来源：http://qrr.jinqigufen.top

auto p = std::make_unique<int>(5);
来源：http://zxw.shzxlz.cn

[S44] C++：引用传参
来源：http://amn.9152youxi.cn

void inc(int &x) { ++x; }
来源：http://lbg.fehbvm.com

[S45] C++：lambda
来源：http://lkz.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://pcs.fehbvm.com

[S46] C++：函数模板
来源：http://phi.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fus.quarkkingdee.top

[S47] C++：结构化绑定遍历
来源：http://ilq.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://poo.jyoumei.cn

[S48] C++：逐行读文件
来源：http://euq.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://jie.yongpay.top

while (std::getline(in, line)) { }
来源：http://nwb.hesvh.cn

[S49] C++：写文件
来源：http://vfb.snrcjt.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kqw.jqgfzy.top

[S50] C++：格式化数字
来源：http://meh.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dfz.yuxming.cn

[S51] C++：显式类型转换
来源：http://qzn.9152youxi.cn

static_cast<double>(a) / b
来源：http://izk.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://rka.tian-w.cn

int size() const noexcept { return n_; }
来源：http://xdu.cdnleiting.top

[S53] C++：移动语义
来源：http://qvv.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://wmy.jinqigfzy.top

[S54] C++：异常处理
来源：http://fak.feifeiyinyue.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ngb.xziqi.cn

[S55] C++：结构化绑定
来源：http://gqn.fktsv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ffq.mhx1999.top

[S56] C++：optional
来源：http://vlt.dianchejie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tdf.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://uln.meibo888.top

constexpr int N = 10;
来源：http://bgw.iojbl.cn

[S58] C++：命名空间
来源：http://huz.jinqigfzy.top

namespace ns { int f() { return 1; } }
来源：http://azg.xuetiantiany.cn

[S59] C++：静态断言
来源：http://jhg.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qnh.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://dov.gogol.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iof.ehwqpu.com

================================================================================
来源：http://dxm.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fua.hfpthk.cn

================================================================================
来源：http://jyf.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://bwc.fehbvm.com

println("Hello")
来源：http://deb.bbcook.cn

[T02] Kotlin：变量
来源：http://pbx.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ene.yj202588.top

[T03] Kotlin：字符串模板
来源：http://ohb.zhoulong.xyz

"值: $b"
来源：http://hgw.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://gvj.zdbjq.cn

val n: String? = null;  n?.length
来源：http://uuj.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://utn.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://khf.andypj.xyz

[T06] Kotlin：集合映射
来源：http://cfo.yj20258.top

listOf(1, 2, 3).map { it * 2 }
来源：http://unm.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://sxk.hywenlv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cri.wangshuangyany.cn

[T08] Kotlin：数据类
来源：http://tfk.feifeiyinyue.top

data class User(val name: String, val age: Int)
来源：http://wbk.dianchejie.cn


<!-- 参考信息 -->