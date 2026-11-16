代发 wailian999

set -euo pipefail
来源：http://zmu.zhijiandao.cn

[R02] 变量赋值与使用
来源：http://pjn.smart0.xyz

name="Tom"; echo "$name"
来源：http://brb.ppjwa.cn

[R03] 只读变量
来源：http://gzw.smart0.xyz

readonly PI=3.14
来源：http://igj.chenzaomai.com

[R04] 位置参数
来源：http://xiw.gaohongyu789.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rqv.hfpthk.cn

[R05] 参数默认值
来源：http://tnl.yangfankeji.com

name="${1:-default}"
来源：http://iyr.iojbl.cn

[R06] 判断命令是否存在
来源：http://ldo.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://obc.gotoacloud.top

[R07] if 判断文件
来源：http://yld.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wvq.zhiwuduotai.top

[R08] 数值比较
来源：http://msr.shanyushiyangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cju.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://sic.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lrc.nanxuanxn.top

[R10] 正则匹配
来源：http://iip.tanke756.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tiu.hesvh.cn

[R11] case 多分支
来源：http://fpp.ydjk.org.cn

case "$1" in
来源：http://gnz.fengsongda.top

start) echo "启动" ;;
来源：http://eng.tianlin.xyz

stop)  echo "停止" ;;
来源：http://cik.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://clg.wangdashe.top

esac
来源：http://jro.yangfankeji.com

[R12] for 遍历文件
来源：http://tfi.pycfn.com

for f in *.txt; do echo "$f"; done
来源：http://izx.redwolf501.top

[R13] for 计数循环
来源：http://tim.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://sxd.fzhhl.top

[R14] C 风格 for
来源：http://klr.shanyushiyangtech.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://atd.zycfv.cn

[R15] while 逐行读文件
来源：http://nhu.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jpa.yvedp.cn

[R16] until 等待条件
来源：http://pwe.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rng.uphjek.com

[R17] 数组定义与取值
来源：http://rja.quarkkingdee.top

arr=(a b c); echo "${arr[0]}"
来源：http://qkx.andypj.xyz

[R18] 遍历数组
来源：http://njn.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aie.aibaodan.cn

[R19] 数组长度
来源：http://rdd.hywenlv.cn

echo "${#arr[@]}"
来源：http://zpk.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://fyv.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://frt.yongpay.top

[R21] 字符串长度
来源：http://peb.nanxinkj.top

echo "${#s}"
来源：http://xdy.zhixingplan.top

[R22] 截取子串
来源：http://xtf.xuetiantiany.cn

echo "${s:0:5}"
来源：http://vin.shuidangran.top

[R23] 字符串替换
来源：http://hhu.hfpthk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sgb.sysykeji.top

[R24] 大小写转换
来源：http://mpe.epnwcf.com

echo "${s^^}"; echo "${s,,}"
来源：http://uag.guowangkeji.top

[R25] 去后缀 / 去前缀
来源：http://gqc.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rip.jianghu66.top

[R26] 命令替换
来源：http://qyc.meibo888.top

now=$(date +%F); echo "$now"
来源：http://ple.jinqigufen.top

[R27] 算术展开
来源：http://lrg.aizwys.cn

echo $((1 + 2 * 3))
来源：http://ebw.gzhubu.top

[R28] 浮点运算
来源：http://adv.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://ecc.zhiwuduotai.top

[R29] 定义函数
来源：http://ytu.zhongyouzk.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mfa.xuanzx.com

[R30] 函数返回状态码
来源：http://jko.jyoumei.cn

f() { return 0; }; f || echo "失败了"
来源：http://zcz.yj202588.top

[R31] 局部变量
来源：http://sjs.hammf.cn

f() { local x=1; echo "$x"; }
来源：http://izt.jlsjyb.cn

[R32] 参数个数校验
来源：http://kgi.epnwcf.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vum.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://rzb.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nwb.shanyushiyangtech.top

[R34] 退出时清理
来源：http://cdy.hongshengwenyu.top

trap 'rm -f "$tmp"' EXIT
来源：http://irm.sjlbkw.cn

[R35] 后台执行并等待
来源：http://kzo.ybcxt.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hou.zhengqikj.top

[R36] 并发执行多个任务
来源：http://hcu.hongshengwenyu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lgp.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://scz.zhaomingkeji.xyz

files=$(ls -1)
来源：http://jzm.sjlbkw.cn

[R38] 管道串联
来源：http://njj.andypj.xyz

cat a.txt | grep -i error | wc -l
来源：http://hyf.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://tyr.yanxiufei.cn

cmd > out.log 2>&1
来源：http://svd.chenzaomai.com

[R40] 追加写日志
来源：http://hhz.ehwqpu.com

echo "log" >> out.log
来源：http://wfr.yvedp.cn

[R41] 丢弃输出
来源：http://aqz.ydjk.org.cn

cmd >/dev/null 2>&1
来源：http://lgt.xziqi.cn

[R42] 输入重定向
来源：http://uxd.uphjek.com

wc -l < a.txt
来源：http://tkc.xinyue.icu

[R43] 按名字查找文件
来源：http://gze.ppjwa.cn

find . -name "*.log" -type f
来源：http://jgp.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://rkn.shzxlz.cn

find . -mtime -7 -type f
来源：http://apx.gogol.net.cn

[R45] 批量删除
来源：http://sxi.yj202588.top

find . -name "*.tmp" -delete
来源：http://gtg.hnqzz.top

[R46] 递归替换文件内容
来源：http://wfn.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://njy.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://fpr.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://lqh.shanyushiyangkeji.top

[R48] awk 取指定列
来源：http://asg.zhiwuduotai.top

awk '{print $1, $3}' a.txt
来源：http://rfq.dianchejie.cn

[R49] awk 带条件
来源：http://nam.shanyushiyangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cfx.hywenlv.cn

[R50] awk 求和
来源：http://mxu.sjlbkw.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zsr.snrcjt.cn

[R51] 排序去重取前几
来源：http://qbf.ppjwa.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dvj.sjlbkw.cn

[R52] 统计行数
来源：http://frg.gogol.net.cn

wc -l a.txt
来源：http://kym.jinqigufen.top

[R53] 查看文件头与实时尾
来源：http://nhy.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uxc.smart0.xyz

[R54] 比较两个文件
来源：http://dua.jqgufenzy.top

diff a.txt b.txt
来源：http://lox.snrcjt.cn

[R55] 压缩与解压
来源：http://mhh.zhengqikj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://erf.ywan-chungtsiang.top

[R56] 远程拷贝
来源：http://wln.bjfxy.top

scp file user@host:/path/
来源：http://zci.sufxvd.cn

[R57] 远程执行命令
来源：http://bar.jyoumei.cn

ssh user@host 'uptime'
来源：http://fji.yvedp.cn

[R58] 下载文件
来源：http://hox.0kj1m.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mtn.redwolf501.top

[R59] 发 POST JSON
来源：http://bky.sxryk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uah.sjlbkw.cn

[R60] 只看 HTTP 状态码
来源：http://dsy.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lvo.andypj.xyz

[R61] 磁盘占用
来源：http://lag.guowangkeji.top

df -h;  du -sh *
来源：http://mqp.hnxiangtu.top

[R62] 找最占空间的文件
来源：http://xgn.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://hxa.yonumen.top

[R63] 内存与进程
来源：http://vcp.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://udy.jiagoushi.top

[R64] 结束进程
来源：http://bug.gogol.net.cn

kill -9 $(pgrep -f app.py)
来源：http://asg.yj20258.top

[R65] 查看端口占用
来源：http://nqu.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yyv.redwolf501.top

[R66] 定时任务
来源：http://dgs.epnwcf.com

crontab -e;  crontab -l
来源：http://dvh.aizwys.cn

[R67] 生成随机十六进制串
来源：http://tun.tianlin.xyz

openssl rand -hex 16
来源：http://zir.yj202588.top

[R68] 计算文件校验值
来源：http://xxw.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jbx.aibaodan.cn

[R69] 生成随机密码
来源：http://qmj.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://put.0kj1m.cn

[R70] 时间戳与互转
来源：http://mqx.xziqi.cn

date +%s;  date -d @1700000000
来源：http://vaa.fktsv.cn

[R71] 日期格式化
来源：http://izy.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xld.cqqwz.cn

[R72] 等待端口就绪
来源：http://uve.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rvt.fehbvm.com

[R73] 分割大日志
来源：http://fki.fktsv.cn

split -l 1000 big.log part_
来源：http://xor.xinyue.icu

[R74] 批量重命名
来源：http://maj.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yvq.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://jis.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://rab.ywan-chungtsiang.top

[R76] 使用临时文件
来源：http://iix.yueranfly.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uop.zhijiandao.cn

[R77] 读取用户输入
来源：http://gvc.tarul.cn

read -rp "请输入: " ans
来源：http://lvv.xinyue.icu

[R78] 交互式菜单
来源：http://hpi.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lay.haohaochexian.top

[R79] 解析命令行选项
来源：http://zcx.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://htb.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://cdv.zhijiandao.cn

time ./run.sh
来源：http://ugf.xuanzx.com

================================================================================
来源：http://gio.zdqjudy.top

S. C / C++ 专题
来源：http://mjs.zhengqikj.top

================================================================================
来源：http://zri.fehbvm.com

[S01] C：Hello World
来源：http://teg.zhoulong.xyz

#include <stdio.h>
来源：http://oeb.shuidangran.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ioq.aizwys.cn

[S02] C：变量与格式化输出
来源：http://hqp.guannengcc.top

int a = 10; printf("%d\n", a);
来源：http://msp.ybcxt.top

[S03] C：读入整数
来源：http://qmq.yj20258.top

int x; scanf("%d", &x);
来源：http://pkn.daria6918.cn

[S04] C：字符串复制
来源：http://pet.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gzd.yfazqb.com

[S05] C：字符串长度
来源：http://qjf.iojbl.cn

strlen(s)
来源：http://wak.mhx1999.top

[S06] C：字符串比较
来源：http://bvi.9152youxi.cn

strcmp(a, b) == 0
来源：http://rbt.kuanghao11.cn

[S07] C：数组遍历求和
来源：http://gcw.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mgj.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://ims.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iop.yj20258.top

[S09] C：结构体定义与初始化
来源：http://ysa.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wfj.jqgufenzy.top

[S10] C：指针与解引用
来源：http://dsv.nanxinkj.top

int *p = &a;  *p = 5;
来源：http://ven.ehwqpu.com

[S11] C：逐行读文件
来源：http://nlb.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://mtz.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://iqo.dianchejie.cn

fclose(f);
来源：http://cvh.jinghuilouyu.cn

[S12] C：写文件
来源：http://swd.fengsongda.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xry.sweek.top

[S13] C：宏定义
来源：http://jot.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ijb.zhixingplan.top

[S14] C：枚举
来源：http://hpn.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://bbj.haohaochexian.top

[S15] C：类型转换
来源：http://uqu.hongshengwenyu.top

(double) a / b
来源：http://obr.feifeiyinyue.top

[S16] C：位操作置位
来源：http://lhx.birdmap.top

x |= (1 << 3);
来源：http://zzb.yuanzhike.top

[S17] C：安全拼接字符串
来源：http://yeh.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://paw.meibo888.top

[S18] C：命令行参数
来源：http://xxf.dianchejie.cn

int main(int argc, char **argv)
来源：http://inl.feifeiyinyue.top

[S19] C：快速排序
来源：http://rlz.fanxiaobao.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://xeh.nwbrower.top

[S20] C：二分查找
来源：http://esh.svipenyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://udc.haohaochexian.top

[S21] C：字符类别判断
来源：http://qgw.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nyq.jianghu66.top

[S22] C：字符串转数字
来源：http://iew.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://xpp.cashguo.top

[S23] C：随机数
来源：http://wuq.fengsongda.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wgi.redwolf501.top

[S24] C：获取本地时间
来源：http://weg.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fbp.yangfankeji.com

[S25] C：内存拷贝
来源：http://zlv.gzhubu.top

memcpy(dst, src, n);
来源：http://fgo.haohaochexian.top

[S26] C：内存清零
来源：http://gcy.316326.xyz

memset(a, 0, sizeof a);
来源：http://efl.zdqjudy.top

[S27] C：定义常量
来源：http://bci.feifeiyinyue.top

const double PI = 3.14159;
来源：http://qmc.yuanzhike.top

[S28] C：静态变量
来源：http://xry.yuxming.cn

static int counter = 0;
来源：http://ttz.zdqjudy.top

[S29] C：变参函数
来源：http://qyr.tarul.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://soz.smart0.xyz

[S30] C：头文件保护
来源：http://eac.xziqi.cn

#ifndef X_H
来源：http://jsf.quarkkingdee.top

#define X_H
来源：http://fvs.zhiwuduotai.top

#endif
来源：http://xit.nanxuanxn.top

[S31] C++：Hello World
来源：http://kej.fktsv.cn

#include <iostream>
来源：http://gww.dianchejie.cn

int main() { std::cout << "Hello\n"; }
来源：http://sqc.cucudq.cn

[S32] C++：字符串
来源：http://cqi.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://wcl.hywenlv.cn

[S33] C++：vector 增删
来源：http://zxq.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zzb.aizwys.cn

[S34] C++：遍历 vector
来源：http://oxu.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://zvy.hysaishi.cn

[S35] C++：map
来源：http://hxl.yongpay.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mgs.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://sgo.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://djh.tarul.cn

[S37] C++：set
来源：http://qgu.ctjpmb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mfa.ctjpmb.com

[S38] C++：排序
来源：http://ter.ehwqpu.com

std::sort(v.begin(), v.end());
来源：http://khn.svipenyu.cn

[S39] C++：自定义比较器排序
来源：http://xzf.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rbm.redwolf501.top

[S40] C++：查找元素
来源：http://bhl.xingfuxueyuan.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rlw.guannengcc.top

[S41] C++：类与构造函数
来源：http://zpy.fzhhl.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jaw.xuetiantiany.cn

[S42] C++：继承与虚函数
来源：http://gfo.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://hda.guowangkeji.top

[S43] C++：智能指针
来源：http://zzl.sysykeji.top

auto p = std::make_unique<int>(5);
来源：http://nve.cashguo.top

[S44] C++：引用传参
来源：http://ulx.xuanzx.com

void inc(int &x) { ++x; }
来源：http://nit.yj202588.top

[S45] C++：lambda
来源：http://rdp.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ivf.yfazqb.com

[S46] C++：函数模板
来源：http://xoi.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hxp.quarkkingdee.top

[S47] C++：结构化绑定遍历
来源：http://qes.hcnkem.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ajn.meibo888.top

[S48] C++：逐行读文件
来源：http://omf.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nvm.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://dvj.jinqigfzy.top

[S49] C++：写文件
来源：http://ijh.jlsjyb.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://doq.hnqzz.top

[S50] C++：格式化数字
来源：http://wsv.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bic.yanxiufei.cn

[S51] C++：显式类型转换
来源：http://lur.xuanzx.com

static_cast<double>(a) / b
来源：http://maa.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://hvx.chenlongwang.top

int size() const noexcept { return n_; }
来源：http://olt.vehdjk.com

[S53] C++：移动语义
来源：http://rxk.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://zvl.fehbvm.com

[S54] C++：异常处理
来源：http://vaz.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tsg.ywan-chungtsiang.top

[S55] C++：结构化绑定
来源：http://drj.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qbl.dashuyun.cn

[S56] C++：optional
来源：http://woj.svipenyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hno.shangyingyoupin.top

[S57] C++：编译期常量
来源：http://swl.zhijiandao.cn

constexpr int N = 10;
来源：http://pdg.sysykeji.top

[S58] C++：命名空间
来源：http://oce.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://iyj.zhixingplan.top

[S59] C++：静态断言
来源：http://lic.xylfe.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pzs.andypj.xyz

[S60] C++：遍历并删除元素
来源：http://snl.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uod.jianghu66.top

================================================================================
来源：http://wgn.c1oappe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lcd.yongpay.top

================================================================================
来源：http://fdr.zhongyouzk.top

[T01] Kotlin：Hello World
来源：http://czw.tanke756.top

println("Hello")
来源：http://cgq.ppjwa.cn

[T02] Kotlin：变量
来源：http://hzy.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qxv.sweek.top


<!-- 参考信息 -->