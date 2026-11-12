代发 wailian999

readonly PI=3.14
来源：http://vdh.zhiwuduotai.top

[R04] 位置参数
来源：http://fmh.yfazqb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://njx.0kj1m.cn

[R05] 参数默认值
来源：http://fgy.sxryk.cn

name="${1:-default}"
来源：http://bbp.hesvh.cn

[R06] 判断命令是否存在
来源：http://exz.shuidangran.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rjx.zhiwuduotai.top

[R07] if 判断文件
来源：http://uvn.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nhb.guowangkeji.top

[R08] 数值比较
来源：http://zwo.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kjq.yj20258888.top

[R09] 字符串比较
来源：http://iup.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sbh.hysaishi.cn

[R10] 正则匹配
来源：http://ady.dianchejie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qvy.jiagoushi.top

[R11] case 多分支
来源：http://smo.shanyushiyangkeji.top

case "$1" in
来源：http://iet.yvedp.cn

start) echo "启动" ;;
来源：http://xcg.jqgufenzy.top

stop)  echo "停止" ;;
来源：http://bca.jinghuilouyu.cn

*)     echo "未知命令" ;;
来源：http://udc.chenzaomai.com

esac
来源：http://rbu.zhongyouzk.top

[R12] for 遍历文件
来源：http://ykw.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://dxn.shzxlz.cn

[R13] for 计数循环
来源：http://kbc.shanyushiyangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://ddv.c1oappe.top

[R14] C 风格 for
来源：http://muo.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ryk.jinqigfzy.top

[R15] while 逐行读文件
来源：http://cfj.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tiu.hongshengwenyu.top

[R16] until 等待条件
来源：http://pwx.gotoacloud.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mff.zhongyouzk.top

[R17] 数组定义与取值
来源：http://aky.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://gaj.zhoulong.xyz

[R18] 遍历数组
来源：http://pwc.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wcj.wangshuangyany.cn

[R19] 数组长度
来源：http://fde.mhx1999.top

echo "${#arr[@]}"
来源：http://aud.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://jsx.daria6918.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vnr.tianlin.xyz

[R21] 字符串长度
来源：http://bhe.dashuyun.cn

echo "${#s}"
来源：http://jrl.nanxuanxn.top

[R22] 截取子串
来源：http://udv.gogol.net.cn

echo "${s:0:5}"
来源：http://tlk.cheryme.top

[R23] 字符串替换
来源：http://gif.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cff.zdbjq.cn

[R24] 大小写转换
来源：http://shp.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ljy.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://ccd.xuetiantiany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ijl.uphjek.com

[R26] 命令替换
来源：http://vhr.aibaodan.cn

now=$(date +%F); echo "$now"
来源：http://xiq.uphjek.com

[R27] 算术展开
来源：http://mca.havefunace.top

echo $((1 + 2 * 3))
来源：http://urc.zycfv.cn

[R28] 浮点运算
来源：http://flu.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://ksf.yuanzhike.top

[R29] 定义函数
来源：http://gwg.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nlf.yangfankeji.com

[R30] 函数返回状态码
来源：http://qhx.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://qzy.yuanzhike.top

[R31] 局部变量
来源：http://qzp.aizwys.cn

f() { local x=1; echo "$x"; }
来源：http://ksy.zycfv.cn

[R32] 参数个数校验
来源：http://oux.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rcx.yueranfly.top

[R33] 捕获错误并提示行号
来源：http://otc.quarkkingdee.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bvr.dashuyun.cn

[R34] 退出时清理
来源：http://yxt.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://upd.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://lpu.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://toq.cheryme.top

[R36] 并发执行多个任务
来源：http://ofc.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qgk.c1oappe.top

[R37] 把输出赋给变量
来源：http://zty.yueranfly.top

files=$(ls -1)
来源：http://hre.jyoumei.cn

[R38] 管道串联
来源：http://sln.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://cvh.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://jpe.sxryk.cn

cmd > out.log 2>&1
来源：http://wco.haohaochexian.top

[R40] 追加写日志
来源：http://moh.tarul.cn

echo "log" >> out.log
来源：http://zbo.xylfe.cn

[R41] 丢弃输出
来源：http://dfy.zhongyouzk.top

cmd >/dev/null 2>&1
来源：http://twr.hesvh.cn

[R42] 输入重定向
来源：http://vny.sufxvd.cn

wc -l < a.txt
来源：http://ydp.ydzc1.top

[R43] 按名字查找文件
来源：http://quy.yanxiufei.cn

find . -name "*.log" -type f
来源：http://iss.xylfe.cn

[R44] 按修改时间查找
来源：http://wkx.vehdjk.com

find . -mtime -7 -type f
来源：http://ctx.zhixingplan.top

[R45] 批量删除
来源：http://kgs.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://ejy.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://apd.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://btj.zdbjq.cn

[R47] sed 单行替换
来源：http://vxc.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://pzj.gaohongyu789.top

[R48] awk 取指定列
来源：http://xzg.daxiang520.top

awk '{print $1, $3}' a.txt
来源：http://cme.tianlin.xyz

[R49] awk 带条件
来源：http://cwc.bjfxy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iar.pengpengdd.cyou

[R50] awk 求和
来源：http://sot.hesvh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bod.xuanzx.com

[R51] 排序去重取前几
来源：http://hej.jlsjyb.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yqf.jinqigufen.top

[R52] 统计行数
来源：http://sal.yvedp.cn

wc -l a.txt
来源：http://aud.feifeiyinyue.top

[R53] 查看文件头与实时尾
来源：http://sih.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pjb.yongpay.top

[R54] 比较两个文件
来源：http://lno.cucudq.cn

diff a.txt b.txt
来源：http://gqc.feifeiyinyue.top

[R55] 压缩与解压
来源：http://ynv.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wkj.zhijiandao.cn

[R56] 远程拷贝
来源：http://lgj.daria6918.cn

scp file user@host:/path/
来源：http://vpq.zhiwuduotai.top

[R57] 远程执行命令
来源：http://unt.xinyue.icu

ssh user@host 'uptime'
来源：http://dpe.shanyushiyangkeji.top

[R58] 下载文件
来源：http://lal.jlsjyb.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://evd.zdbjq.cn

[R59] 发 POST JSON
来源：http://wgr.fktsv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gbq.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://jdi.cqqwz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jqc.9152youxi.cn

[R61] 磁盘占用
来源：http://gqq.jqgufenzy.top

df -h;  du -sh *
来源：http://jtm.ydzc1.top

[R62] 找最占空间的文件
来源：http://krd.xuanzx.com

du -ah . | sort -rh | head -10
来源：http://oxc.ybcxt.top

[R63] 内存与进程
来源：http://ujm.gogol.net.cn

free -h;  ps aux | grep nginx
来源：http://cps.xylfe.cn

[R64] 结束进程
来源：http://feh.bbcook.cn

kill -9 $(pgrep -f app.py)
来源：http://ybw.gaohongyu789.top

[R65] 查看端口占用
来源：http://xdk.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yzm.havefunace.top

[R66] 定时任务
来源：http://ebq.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://pfk.cqqwz.cn

[R67] 生成随机十六进制串
来源：http://cnm.dashuyun.cn

openssl rand -hex 16
来源：http://qmm.gotoacloud.top

[R68] 计算文件校验值
来源：http://avx.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gvq.hcnkem.com

[R69] 生成随机密码
来源：http://yzc.meibo888.top

head -c 16 /dev/urandom | base64
来源：http://qfu.daria6918.cn

[R70] 时间戳与互转
来源：http://xpt.hcnkem.com

date +%s;  date -d @1700000000
来源：http://dug.daria6918.cn

[R71] 日期格式化
来源：http://szi.cqqwz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bqn.fehbvm.com

[R72] 等待端口就绪
来源：http://ztq.nwbrower.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mrm.vqdsnc.cn

[R73] 分割大日志
来源：http://cjz.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://qfc.fengsongda.top

[R74] 批量重命名
来源：http://udd.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rim.jianghu66.top

[R75] 导出环境变量
来源：http://nxz.tanke756.top

export PATH="$HOME/bin:$PATH"
来源：http://wnn.316326.xyz

[R76] 使用临时文件
来源：http://uhy.jlsjyb.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://omq.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://gap.fehbvm.com

read -rp "请输入: " ans
来源：http://vxh.9152youxi.cn

[R78] 交互式菜单
来源：http://psd.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zcq.jianghu66.top

[R79] 解析命令行选项
来源：http://ybz.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ivy.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://phk.shzxlz.cn

time ./run.sh
来源：http://lvx.cqqwz.cn

================================================================================
来源：http://dee.shzxlz.cn

S. C / C++ 专题
来源：http://cqr.bjfxy.top

================================================================================
来源：http://mev.hysaishi.cn

[S01] C：Hello World
来源：http://qrm.hnqzz.top

#include <stdio.h>
来源：http://uub.jlsjyb.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hnq.nanxuanxn.top

[S02] C：变量与格式化输出
来源：http://bsp.wangdashe.top

int a = 10; printf("%d\n", a);
来源：http://tam.zhijiandao.cn

[S03] C：读入整数
来源：http://tza.sysykeji.top

int x; scanf("%d", &x);
来源：http://xyt.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://zku.shangyingyoupin.top

char dst[32]; strcpy(dst, "hi");
来源：http://gcx.tian-w.cn

[S05] C：字符串长度
来源：http://cnq.hnxiangtu.top

strlen(s)
来源：http://xbx.yuxming.cn

[S06] C：字符串比较
来源：http://cup.pengpengdd.cyou

strcmp(a, b) == 0
来源：http://atb.hammf.cn

[S07] C：数组遍历求和
来源：http://vmx.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ixk.sweek.top

[S08] C：动态内存分配与释放
来源：http://mdf.yueranfly.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ntf.yvedp.cn

[S09] C：结构体定义与初始化
来源：http://zzo.mhx1999.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nii.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://skh.ivvv.top

int *p = &a;  *p = 5;
来源：http://you.yfazqb.com

[S11] C：逐行读文件
来源：http://ewb.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://mjr.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://gpo.yonumen.top

fclose(f);
来源：http://jfv.hcnkem.com

[S12] C：写文件
来源：http://tkl.bbcook.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tck.jinghuilouyu.cn

[S13] C：宏定义
来源：http://fyc.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rsu.jinghuilouyu.cn

[S14] C：枚举
来源：http://jfu.zdbjq.cn

enum Color { RED, GREEN, BLUE };
来源：http://hpn.yueranfly.top

[S15] C：类型转换
来源：http://wzp.zhoulong.xyz

(double) a / b
来源：http://hsk.zhixingplan.top

[S16] C：位操作置位
来源：http://xvn.sysykeji.top

x |= (1 << 3);
来源：http://ujh.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://zpc.yuanzhike.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tbo.jiagoushi.top

[S18] C：命令行参数
来源：http://nmt.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://eex.sjlbkw.cn

[S19] C：快速排序
来源：http://blg.guannengcc.top

qsort(a, n, sizeof(int), cmp);
来源：http://waf.316326.xyz

[S20] C：二分查找
来源：http://rbs.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qwm.sysykeji.top

[S21] C：字符类别判断
来源：http://ugd.vehdjk.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gyh.jyoumei.cn

[S22] C：字符串转数字
来源：http://dcg.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://vgv.gotoacloud.top

[S23] C：随机数
来源：http://wpu.cdnleiting.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zwc.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://tor.wangshuangyany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://agf.ydjk.org.cn

[S25] C：内存拷贝
来源：http://plt.ydjk.org.cn

memcpy(dst, src, n);
来源：http://siw.jyoumei.cn

[S26] C：内存清零
来源：http://sjl.andypj.xyz

memset(a, 0, sizeof a);
来源：http://tzo.fengsongda.top

[S27] C：定义常量
来源：http://smm.yfazqb.com

const double PI = 3.14159;
来源：http://ary.wangdashe.top

[S28] C：静态变量
来源：http://oqc.nanxuanxn.top

static int counter = 0;
来源：http://hvx.zhongyouzk.top

[S29] C：变参函数
来源：http://mic.jqgfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xma.chenlongwang.top

[S30] C：头文件保护
来源：http://itr.yanxiufei.cn

#ifndef X_H
来源：http://dhc.chenlongwang.top

#define X_H
来源：http://isb.xingfuxueyuan.xyz

#endif
来源：http://oob.fengsongda.top

[S31] C++：Hello World
来源：http://ops.feifeiyinyue.top

#include <iostream>
来源：http://alo.zycfv.cn

int main() { std::cout << "Hello\n"; }
来源：http://blm.yangfankeji.com

[S32] C++：字符串
来源：http://bgs.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://kzv.fengsongda.top

[S33] C++：vector 增删
来源：http://ute.epnwcf.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://enu.xziqi.cn

[S34] C++：遍历 vector
来源：http://lvv.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://fri.uphjek.com

[S35] C++：map
来源：http://ory.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vso.hnqzz.top

[S36] C++：unordered_map
来源：http://fag.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xea.yvedp.cn

[S37] C++：set
来源：http://jwg.ctjpmb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nir.uphjek.com

[S38] C++：排序
来源：http://dpj.52xcode.cn

std::sort(v.begin(), v.end());
来源：http://eie.zhiwuduotai.top

[S39] C++：自定义比较器排序
来源：http://tzs.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kma.tianlin.xyz

[S40] C++：查找元素
来源：http://jrq.fengsongda.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ioj.guannengcc.top

[S41] C++：类与构造函数
来源：http://ajz.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gcn.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://cqy.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://jce.hcnkem.com

[S43] C++：智能指针
来源：http://mpv.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://vmk.xylfe.cn

[S44] C++：引用传参
来源：http://omt.dashuyun.cn

void inc(int &x) { ++x; }
来源：http://yfj.bjfxy.top

[S45] C++：lambda
来源：http://suc.zhoulong.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://frp.sufxvd.cn

[S46] C++：函数模板
来源：http://gfa.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uim.tanke756.top

[S47] C++：结构化绑定遍历
来源：http://dsc.yueranfly.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pss.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://nwp.nwbrower.top

std::ifstream in("a.txt");  std::string line;
来源：http://awu.havefunace.top

while (std::getline(in, line)) { }
来源：http://gai.pycfn.com

[S49] C++：写文件
来源：http://fqi.svipenyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fgu.xziqi.cn

[S50] C++：格式化数字
来源：http://jak.tarul.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gwy.hesvh.cn

[S51] C++：显式类型转换
来源：http://klq.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://esp.svipenyu.cn

[S52] C++：const 与 noexcept
来源：http://bpr.fktsv.cn

int size() const noexcept { return n_; }
来源：http://gow.jlsjyb.cn

[S53] C++：移动语义
来源：http://xle.quarkkingdee.top

std::vector<int> w = std::move(v);
来源：http://ocv.ydjk.org.cn

[S54] C++：异常处理
来源：http://euq.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vkh.fengsongda.top

[S55] C++：结构化绑定
来源：http://rqe.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bgj.yuxming.cn

[S56] C++：optional
来源：http://mnh.hnxiangtu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pbu.shanyushiyangtech.top

[S57] C++：编译期常量
来源：http://ach.cucudq.cn

constexpr int N = 10;
来源：http://ogp.c1oappe.top

[S58] C++：命名空间
来源：http://seu.hywenlv.cn

namespace ns { int f() { return 1; } }
来源：http://vie.fehbvm.com

[S59] C++：静态断言
来源：http://muu.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xfe.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://fvj.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kyb.ivvv.top

================================================================================
来源：http://kod.nanxinkj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gfr.nanxinkj.top

================================================================================
来源：http://bum.jinqigufen.top

[T01] Kotlin：Hello World
来源：http://rrp.ywan-chungtsiang.top

println("Hello")
来源：http://inr.iojbl.cn

[T02] Kotlin：变量
来源：http://qpi.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uvn.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://mjg.zdqjudy.top

"值: $b"
来源：http://qcs.hesvh.cn

[T04] Kotlin：空安全
来源：http://eum.feifeiyinyue.top

val n: String? = null;  n?.length
来源：http://nlu.ppjwa.cn


<!-- 参考信息 -->