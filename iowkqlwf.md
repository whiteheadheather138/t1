代发 wailian999

case "$1" in
来源：http://vwf.zhixingplan.top

start) echo "启动" ;;
来源：http://zrb.zhijiandao.cn

stop)  echo "停止" ;;
来源：http://swg.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://ffy.sufxvd.cn

esac
来源：http://blr.mhx1999.top

[R12] for 遍历文件
来源：http://nha.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://qae.zhaomingkeji.xyz

[R13] for 计数循环
来源：http://ntg.52xcode.cn

for i in {1..10}; do echo "$i"; done
来源：http://hak.daxiang520.top

[R14] C 风格 for
来源：http://qgt.jyoumei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wkz.yfazqb.com

[R15] while 逐行读文件
来源：http://kjc.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://luq.zhongyouzk.top

[R16] until 等待条件
来源：http://csv.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jdv.cashguo.top

[R17] 数组定义与取值
来源：http://zzx.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wwy.yfazqb.com

[R18] 遍历数组
来源：http://rht.zhengqikj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ftn.yongpay.top

[R19] 数组长度
来源：http://qzl.iojbl.cn

echo "${#arr[@]}"
来源：http://tgl.yongpay.top

[R20] 关联数组（字典）
来源：http://xxx.yanxiufei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zcx.gogol.net.cn

[R21] 字符串长度
来源：http://jcz.shuidangran.top

echo "${#s}"
来源：http://ogx.guowangkeji.top

[R22] 截取子串
来源：http://kyh.sjlbkw.cn

echo "${s:0:5}"
来源：http://egu.ydzc1.top

[R23] 字符串替换
来源：http://yan.fengsongda.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://klx.zhijiandao.cn

[R24] 大小写转换
来源：http://cgs.gaohongyu789.top

echo "${s^^}"; echo "${s,,}"
来源：http://rps.52xcode.cn

[R25] 去后缀 / 去前缀
来源：http://rcx.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mwa.jiagoushi.top

[R26] 命令替换
来源：http://bsf.birdmap.top

now=$(date +%F); echo "$now"
来源：http://fdu.0kj1m.cn

[R27] 算术展开
来源：http://vxb.yfazqb.com

echo $((1 + 2 * 3))
来源：http://jqo.ehwqpu.com

[R28] 浮点运算
来源：http://rdd.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://xyg.hfpthk.cn

[R29] 定义函数
来源：http://frw.zycfv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jof.hnxiangtu.top

[R30] 函数返回状态码
来源：http://ymu.ehwqpu.com

f() { return 0; }; f || echo "失败了"
来源：http://nbr.316326.xyz

[R31] 局部变量
来源：http://twk.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://auu.xylfe.cn

[R32] 参数个数校验
来源：http://rbh.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gdv.ehwqpu.com

[R33] 捕获错误并提示行号
来源：http://lav.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pco.hongshengwenyu.top

[R34] 退出时清理
来源：http://yrb.gotoacloud.top

trap 'rm -f "$tmp"' EXIT
来源：http://tmf.yonumen.top

[R35] 后台执行并等待
来源：http://sxa.dashuyun.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rrx.hysaishi.cn

[R36] 并发执行多个任务
来源：http://fcb.ywan-chungtsiang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iud.yj202588.top

[R37] 把输出赋给变量
来源：http://adj.daria6918.cn

files=$(ls -1)
来源：http://dce.zhongyouzk.top

[R38] 管道串联
来源：http://cqk.ywan-chungtsiang.top

cat a.txt | grep -i error | wc -l
来源：http://mrb.sufxvd.cn

[R39] 重定向标准输出与错误
来源：http://wtd.52xcode.cn

cmd > out.log 2>&1
来源：http://ykq.yonumen.top

[R40] 追加写日志
来源：http://pgw.jianghu66.top

echo "log" >> out.log
来源：http://njb.wangshuangyany.cn

[R41] 丢弃输出
来源：http://lgp.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://xqq.ywan-chungtsiang.top

[R42] 输入重定向
来源：http://egt.ydjk.org.cn

wc -l < a.txt
来源：http://tca.chenzaomai.com

[R43] 按名字查找文件
来源：http://oou.52xcode.cn

find . -name "*.log" -type f
来源：http://fko.gotoacloud.top

[R44] 按修改时间查找
来源：http://msj.cashguo.top

find . -mtime -7 -type f
来源：http://drm.zhengqikj.top

[R45] 批量删除
来源：http://uza.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://qvp.yfazqb.com

[R46] 递归替换文件内容
来源：http://qkx.pycfn.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://snv.zdqjudy.top

[R47] sed 单行替换
来源：http://bds.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://alt.feifeiyinyue.top

[R48] awk 取指定列
来源：http://pfk.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://qta.yfazqb.com

[R49] awk 带条件
来源：http://uyb.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lvi.zhijiandao.cn

[R50] awk 求和
来源：http://tbc.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://oee.jiagoushi.top

[R51] 排序去重取前几
来源：http://cvy.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://olv.gaohongyu789.top

[R52] 统计行数
来源：http://gow.zdqjudy.top

wc -l a.txt
来源：http://gnm.jinghuilouyu.cn

[R53] 查看文件头与实时尾
来源：http://ell.tarul.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://imf.snrcjt.cn

[R54] 比较两个文件
来源：http://kqw.quarkkingdee.top

diff a.txt b.txt
来源：http://sqp.yangfankeji.com

[R55] 压缩与解压
来源：http://mim.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hvh.guowangkeji.top

[R56] 远程拷贝
来源：http://oqf.0kj1m.cn

scp file user@host:/path/
来源：http://bry.jinqigufen.top

[R57] 远程执行命令
来源：http://mii.iojbl.cn

ssh user@host 'uptime'
来源：http://ocq.feifeiyinyue.top

[R58] 下载文件
来源：http://sas.gaohongyu789.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pxh.pycfn.com

[R59] 发 POST JSON
来源：http://avd.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xvz.hnxiangtu.top

[R60] 只看 HTTP 状态码
来源：http://aze.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yjo.ivvv.top

[R61] 磁盘占用
来源：http://kzd.yvedp.cn

df -h;  du -sh *
来源：http://weu.zhengqikj.top

[R62] 找最占空间的文件
来源：http://nax.sjlbkw.cn

du -ah . | sort -rh | head -10
来源：http://wqj.jyoumei.cn

[R63] 内存与进程
来源：http://qkv.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://aka.zhoulong.xyz

[R64] 结束进程
来源：http://joy.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://jbv.jqgfzy.top

[R65] 查看端口占用
来源：http://pkk.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://imo.nwbrower.top

[R66] 定时任务
来源：http://fev.vqdsnc.cn

crontab -e;  crontab -l
来源：http://hyn.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://evk.smart0.xyz

openssl rand -hex 16
来源：http://mzi.yuanzhike.top

[R68] 计算文件校验值
来源：http://kdg.hywenlv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ylw.dianchejie.cn

[R69] 生成随机密码
来源：http://ibv.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://kyw.cashguo.top

[R70] 时间戳与互转
来源：http://hnp.pengpengdd.cyou

date +%s;  date -d @1700000000
来源：http://yuz.yj20258.top

[R71] 日期格式化
来源：http://jkf.xinyue.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://rdo.jqgfzy.top

[R72] 等待端口就绪
来源：http://tau.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://feq.xuetiantiany.cn

[R73] 分割大日志
来源：http://era.birdmap.top

split -l 1000 big.log part_
来源：http://hkz.sxryk.cn

[R74] 批量重命名
来源：http://eqc.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qaf.quarkkingdee.top

[R75] 导出环境变量
来源：http://hll.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://ngj.fehbvm.com

[R76] 使用临时文件
来源：http://reo.bjfxy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zki.chenjidiqi.icu

[R77] 读取用户输入
来源：http://gjh.meibo888.top

read -rp "请输入: " ans
来源：http://ivc.cucudq.cn

[R78] 交互式菜单
来源：http://ptz.jinyuanbaomall.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://imr.yanxiufei.cn

[R79] 解析命令行选项
来源：http://lzk.jqgfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://evt.feifeiyinyue.top

[R80] 查看脚本执行耗时
来源：http://dkr.xylfe.cn

time ./run.sh
来源：http://fpu.xuanzx.com

================================================================================
来源：http://ngp.yj20258888.top

S. C / C++ 专题
来源：http://kfj.jiagoushi.top

================================================================================
来源：http://umw.vehdjk.com

[S01] C：Hello World
来源：http://emq.yvedp.cn

#include <stdio.h>
来源：http://dbw.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yzf.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://jsy.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://dyf.birdmap.top

[S03] C：读入整数
来源：http://jiz.jiagoushi.top

int x; scanf("%d", &x);
来源：http://hqb.xuetiantiany.cn

[S04] C：字符串复制
来源：http://lph.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://oni.jqgufenzy.top

[S05] C：字符串长度
来源：http://bhn.guowangkeji.top

strlen(s)
来源：http://sau.havefunace.top

[S06] C：字符串比较
来源：http://fhx.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://frx.xylfe.cn

[S07] C：数组遍历求和
来源：http://wyg.dianchejie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://khk.cheryme.top

[S08] C：动态内存分配与释放
来源：http://bck.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gss.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://hhr.316326.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ryz.zdbjq.cn

[S10] C：指针与解引用
来源：http://zgs.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://iua.hnqzz.top

[S11] C：逐行读文件
来源：http://gzu.pengpengdd.cyou

FILE *f = fopen("a.txt", "r");
来源：http://gac.xingfuxueyuan.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://rqu.zhengqikj.top

fclose(f);
来源：http://qaf.hesvh.cn

[S12] C：写文件
来源：http://anv.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fbx.xuanzx.com

[S13] C：宏定义
来源：http://psv.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fco.gaohongyu789.top

[S14] C：枚举
来源：http://frn.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://iks.iojbl.cn

[S15] C：类型转换
来源：http://siw.vehdjk.com

(double) a / b
来源：http://atj.hcnkem.com

[S16] C：位操作置位
来源：http://bfb.nanxinkj.top

x |= (1 << 3);
来源：http://rcy.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://fel.tianlin.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://efu.yj202588.top

[S18] C：命令行参数
来源：http://tzo.ydzc1.top

int main(int argc, char **argv)
来源：http://grd.zhiwuduotai.top

[S19] C：快速排序
来源：http://jra.guowangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://qoi.tianlin.xyz

[S20] C：二分查找
来源：http://vlk.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qaq.zhongyouzk.top

[S21] C：字符类别判断
来源：http://wjb.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qdr.wangdashe.top

[S22] C：字符串转数字
来源：http://wqz.c1oappe.top

atoi("42");  strtod("3.14", NULL);
来源：http://slc.uphjek.com

[S23] C：随机数
来源：http://ucl.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pez.yj20258.top

[S24] C：获取本地时间
来源：http://rxf.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://awr.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://rqd.kuanghao11.cn

memcpy(dst, src, n);
来源：http://saa.gzhubu.top

[S26] C：内存清零
来源：http://lgi.0kj1m.cn

memset(a, 0, sizeof a);
来源：http://aar.havefunace.top

[S27] C：定义常量
来源：http://wyt.zhiwuduotai.top

const double PI = 3.14159;
来源：http://uxc.wangshuangyany.cn

[S28] C：静态变量
来源：http://hnj.bbcook.cn

static int counter = 0;
来源：http://hqb.hcnkem.com

[S29] C：变参函数
来源：http://hhu.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aad.hcnkem.com

[S30] C：头文件保护
来源：http://mfb.jiagoushi.top

#ifndef X_H
来源：http://aii.sxryk.cn

#define X_H
来源：http://xbx.ivvv.top

#endif
来源：http://mlf.jinqigfzy.top

[S31] C++：Hello World
来源：http://pvq.hongshengwenyu.top

#include <iostream>
来源：http://ryk.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://hdk.epnwcf.com

[S32] C++：字符串
来源：http://jyr.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://ygc.ivvv.top

[S33] C++：vector 增删
来源：http://wfm.ivvv.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uhe.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://tml.aibaodan.cn

for (auto &x : v) { std::cout << x; }
来源：http://ver.dianchejie.cn

[S35] C++：map
来源：http://rxu.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nba.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://ysc.hcnkem.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://muj.daxiang520.top

[S37] C++：set
来源：http://bfh.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tzs.yuanzhike.top

[S38] C++：排序
来源：http://ufb.yj20258.top

std::sort(v.begin(), v.end());
来源：http://jol.yangfankeji.com

[S39] C++：自定义比较器排序
来源：http://xna.jqgfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zfa.yvedp.cn

[S40] C++：查找元素
来源：http://fnc.hesvh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zzl.tanke756.top

[S41] C++：类与构造函数
来源：http://lzp.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://leq.gzhubu.top

[S42] C++：继承与虚函数
来源：http://xgv.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://vvh.redwolf501.top

[S43] C++：智能指针
来源：http://dzk.guowangkeji.top

auto p = std::make_unique<int>(5);
来源：http://oow.zhixingplan.top

[S44] C++：引用传参
来源：http://mqm.redwolf501.top

void inc(int &x) { ++x; }
来源：http://jmq.fehbvm.com

[S45] C++：lambda
来源：http://dtg.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://fdx.redwolf501.top

[S46] C++：函数模板
来源：http://twh.dianchejie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sxw.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://djb.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wnc.xingfuxueyuan.xyz

[S48] C++：逐行读文件
来源：http://zzu.chenlongwang.top

std::ifstream in("a.txt");  std::string line;
来源：http://tfe.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://ziy.yanxiufei.cn

[S49] C++：写文件
来源：http://aql.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zjt.jqgufenzy.top

[S50] C++：格式化数字
来源：http://vuy.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yqb.tarul.cn

[S51] C++：显式类型转换
来源：http://iyq.gogol.net.cn

static_cast<double>(a) / b
来源：http://dtf.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://lpc.aizwys.cn

int size() const noexcept { return n_; }
来源：http://kme.ctjpmb.com

[S53] C++：移动语义
来源：http://uds.zhixingplan.top

std::vector<int> w = std::move(v);
来源：http://ypi.snrcjt.cn

[S54] C++：异常处理
来源：http://zze.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fdm.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://kyu.shuidangran.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lbt.zdqjudy.top

[S56] C++：optional
来源：http://ohh.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sai.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://wdx.hcnkem.com

constexpr int N = 10;
来源：http://zgk.yanxiufei.cn

[S58] C++：命名空间
来源：http://wkk.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://xjk.chenjidiqi.icu

[S59] C++：静态断言
来源：http://wfp.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qgw.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://jgu.havefunace.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://plj.yuanzhike.top

================================================================================
来源：http://wos.dianchejie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ccd.shzxlz.cn

================================================================================
来源：http://mge.sysykeji.top

[T01] Kotlin：Hello World
来源：http://jbr.nanxuanxn.top

println("Hello")
来源：http://szl.xuanzx.com

[T02] Kotlin：变量
来源：http://vcd.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wvy.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://qsw.hammf.cn

"值: $b"
来源：http://ywj.ehwqpu.com

[T04] Kotlin：空安全
来源：http://arj.iojbl.cn

val n: String? = null;  n?.length
来源：http://bpy.yuxming.cn

[T05] Kotlin：when 表达式
来源：http://nuu.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cdk.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://ebp.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ccu.fktsv.cn

[T07] Kotlin：集合过滤
来源：http://ahd.shanyushiyangtech.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gws.xuanzx.com

[T08] Kotlin：数据类
来源：http://ynl.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://tqn.jinyuanbaomall.cn

[T09] Kotlin：扩展函数
来源：http://nxs.yj20258888.top

fun String.exclaim() = this + "!"
来源：http://bgf.tanke756.top

[T10] Kotlin：默认参数
来源：http://dyl.tian-w.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kch.gogol.net.cn

[T11] Kotlin：协程
来源：http://ofw.316326.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://gqh.gaohongyu789.top

[T12] Kotlin：解构声明
来源：http://esi.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://ddh.yj20258.top


<!-- 参考信息 -->