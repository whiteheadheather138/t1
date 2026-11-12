代发 wailian999

case "$1" in
来源：http://nck.ybcxt.top

start) echo "启动" ;;
来源：http://rai.hesvh.cn

stop)  echo "停止" ;;
来源：http://ijz.xuetiantiany.cn

*)     echo "未知命令" ;;
来源：http://rnr.jlsjyb.cn

esac
来源：http://yid.hammf.cn

[R12] for 遍历文件
来源：http://lnr.cucudq.cn

for f in *.txt; do echo "$f"; done
来源：http://uhn.zhaomingkeji.xyz

[R13] for 计数循环
来源：http://ykl.gaohongyu789.top

for i in {1..10}; do echo "$i"; done
来源：http://zmj.daria6918.cn

[R14] C 风格 for
来源：http://onk.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iqz.andypj.xyz

[R15] while 逐行读文件
来源：http://vtq.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uup.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://olw.zhaomingkeji.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nem.yueranfly.top

[R17] 数组定义与取值
来源：http://kyf.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://luo.fengsongda.top

[R18] 遍历数组
来源：http://vtf.gaohongyu789.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tub.yj202588.top

[R19] 数组长度
来源：http://efg.shanyushiyangtech.top

echo "${#arr[@]}"
来源：http://tuh.zdqjudy.top

[R20] 关联数组（字典）
来源：http://trn.dianchejie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tcg.yanxiufei.cn

[R21] 字符串长度
来源：http://xsz.zdbjq.cn

echo "${#s}"
来源：http://zdu.yonumen.top

[R22] 截取子串
来源：http://mbi.c1oappe.top

echo "${s:0:5}"
来源：http://lnw.xuanzx.com

[R23] 字符串替换
来源：http://aly.nwbrower.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://twm.yj20258888.top

[R24] 大小写转换
来源：http://frt.guannengcc.top

echo "${s^^}"; echo "${s,,}"
来源：http://vbi.mhx1999.top

[R25] 去后缀 / 去前缀
来源：http://xcb.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://twt.mhx1999.top

[R26] 命令替换
来源：http://ghf.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://wrv.shanyushiyangtech.top

[R27] 算术展开
来源：http://fro.shanyushiyangtech.top

echo $((1 + 2 * 3))
来源：http://cxd.ybcxt.top

[R28] 浮点运算
来源：http://ldj.aizwys.cn

echo "scale=2; 10/3" | bc
来源：http://qie.andypj.xyz

[R29] 定义函数
来源：http://yig.dianchejie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nba.andypj.xyz

[R30] 函数返回状态码
来源：http://mvc.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://bel.iojbl.cn

[R31] 局部变量
来源：http://ufn.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://umj.redwolf501.top

[R32] 参数个数校验
来源：http://yib.ywan-chungtsiang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ali.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://qkd.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hmv.dianchejie.cn

[R34] 退出时清理
来源：http://bmq.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://yua.gaohongyu789.top

[R35] 后台执行并等待
来源：http://ahe.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://wui.svipenyu.cn

[R36] 并发执行多个任务
来源：http://iqm.ydjk.org.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uks.yuanzhike.top

[R37] 把输出赋给变量
来源：http://igy.xuanzx.com

files=$(ls -1)
来源：http://hnt.ivvv.top

[R38] 管道串联
来源：http://mtr.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://xwk.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://evf.hfpthk.cn

cmd > out.log 2>&1
来源：http://cjh.fzhhl.top

[R40] 追加写日志
来源：http://kqc.sjlbkw.cn

echo "log" >> out.log
来源：http://zwx.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://hkw.ydjk.org.cn

cmd >/dev/null 2>&1
来源：http://gpr.dianchejie.cn

[R42] 输入重定向
来源：http://xwa.0kj1m.cn

wc -l < a.txt
来源：http://ump.xylfe.cn

[R43] 按名字查找文件
来源：http://fgi.wangdashe.top

find . -name "*.log" -type f
来源：http://iew.zhengqikj.top

[R44] 按修改时间查找
来源：http://yeq.iojbl.cn

find . -mtime -7 -type f
来源：http://tzj.yvedp.cn

[R45] 批量删除
来源：http://enw.52xcode.cn

find . -name "*.tmp" -delete
来源：http://gzg.xylfe.cn

[R46] 递归替换文件内容
来源：http://jsr.birdmap.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qnw.gaohongyu789.top

[R47] sed 单行替换
来源：http://hah.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://pmr.gotoacloud.top

[R48] awk 取指定列
来源：http://fdn.sxryk.cn

awk '{print $1, $3}' a.txt
来源：http://eok.yanxiufei.cn

[R49] awk 带条件
来源：http://tpu.xuetiantiany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uqb.fengsongda.top

[R50] awk 求和
来源：http://syt.jqgufenzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://ldd.kuanghao11.cn

[R51] 排序去重取前几
来源：http://shd.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://esf.dianchejie.cn

[R52] 统计行数
来源：http://zqk.ydzc1.top

wc -l a.txt
来源：http://liq.zhaomingkeji.xyz

[R53] 查看文件头与实时尾
来源：http://pgq.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qml.aizwys.cn

[R54] 比较两个文件
来源：http://hhx.ydzc1.top

diff a.txt b.txt
来源：http://qfu.fktsv.cn

[R55] 压缩与解压
来源：http://pdc.sufxvd.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vdv.jiagoushi.top

[R56] 远程拷贝
来源：http://itx.quarkkingdee.top

scp file user@host:/path/
来源：http://jeg.quarkkingdee.top

[R57] 远程执行命令
来源：http://vmq.yangfankeji.com

ssh user@host 'uptime'
来源：http://eqp.zhaomingkeji.xyz

[R58] 下载文件
来源：http://htq.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://thn.zdbjq.cn

[R59] 发 POST JSON
来源：http://hea.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nrd.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://lwd.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eib.chenjidiqi.icu

[R61] 磁盘占用
来源：http://fqx.fktsv.cn

df -h;  du -sh *
来源：http://exz.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://kse.uphjek.com

du -ah . | sort -rh | head -10
来源：http://dfx.zhixingplan.top

[R63] 内存与进程
来源：http://lmh.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://tci.ehwqpu.com

[R64] 结束进程
来源：http://klh.zdbjq.cn

kill -9 $(pgrep -f app.py)
来源：http://frf.52xcode.cn

[R65] 查看端口占用
来源：http://ynw.hysaishi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jgw.jiagoushi.top

[R66] 定时任务
来源：http://kgf.cheryme.top

crontab -e;  crontab -l
来源：http://awz.yuanzhike.top

[R67] 生成随机十六进制串
来源：http://mzl.birdmap.top

openssl rand -hex 16
来源：http://xht.cucudq.cn

[R68] 计算文件校验值
来源：http://brq.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://gws.yj20258888.top

[R69] 生成随机密码
来源：http://enz.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://oaw.yanxiufei.cn

[R70] 时间戳与互转
来源：http://ajg.shangyingyoupin.top

date +%s;  date -d @1700000000
来源：http://aro.smart0.xyz

[R71] 日期格式化
来源：http://igu.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bst.cheryme.top

[R72] 等待端口就绪
来源：http://ros.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xae.gaohongyu789.top

[R73] 分割大日志
来源：http://xys.yuxming.cn

split -l 1000 big.log part_
来源：http://hyo.ydjk.org.cn

[R74] 批量重命名
来源：http://etk.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wlx.jlsjyb.cn

[R75] 导出环境变量
来源：http://fhx.tarul.cn

export PATH="$HOME/bin:$PATH"
来源：http://svl.cucudq.cn

[R76] 使用临时文件
来源：http://xrz.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oqc.hongshengwenyu.top

[R77] 读取用户输入
来源：http://xbn.tianlin.xyz

read -rp "请输入: " ans
来源：http://ngy.pycfn.com

[R78] 交互式菜单
来源：http://jwm.chenlongwang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jxb.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://wcl.xylfe.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://abl.vehdjk.com

[R80] 查看脚本执行耗时
来源：http://llv.c1oappe.top

time ./run.sh
来源：http://iis.cheryme.top

================================================================================
来源：http://oci.dashuyun.cn

S. C / C++ 专题
来源：http://aes.hcnkem.com

================================================================================
来源：http://llm.jiagoushi.top

[S01] C：Hello World
来源：http://uzg.zycfv.cn

#include <stdio.h>
来源：http://mjb.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xmh.hesvh.cn

[S02] C：变量与格式化输出
来源：http://cew.shuidangran.top

int a = 10; printf("%d\n", a);
来源：http://oqf.guannengcc.top

[S03] C：读入整数
来源：http://eym.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://ffw.yj20258888.top

[S04] C：字符串复制
来源：http://bmg.aizwys.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dwi.birdmap.top

[S05] C：字符串长度
来源：http://gww.chenzaomai.com

strlen(s)
来源：http://nih.xuanzx.com

[S06] C：字符串比较
来源：http://kau.bbcook.cn

strcmp(a, b) == 0
来源：http://srx.yanxiufei.cn

[S07] C：数组遍历求和
来源：http://xzr.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bzs.sufxvd.cn

[S08] C：动态内存分配与释放
来源：http://ebq.mhx1999.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vom.guowangkeji.top

[S09] C：结构体定义与初始化
来源：http://nlq.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://opq.9152youxi.cn

[S10] C：指针与解引用
来源：http://nhy.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://ezx.aizwys.cn

[S11] C：逐行读文件
来源：http://mbe.tanke756.top

FILE *f = fopen("a.txt", "r");
来源：http://hdc.mhx1999.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kqh.dashuyun.cn

fclose(f);
来源：http://qfh.316326.xyz

[S12] C：写文件
来源：http://wod.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sqk.hnqzz.top

[S13] C：宏定义
来源：http://hjd.svipenyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vmo.nwbrower.top

[S14] C：枚举
来源：http://bly.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://xym.tian-w.cn

[S15] C：类型转换
来源：http://pzm.birdmap.top

(double) a / b
来源：http://sdu.hongshengwenyu.top

[S16] C：位操作置位
来源：http://fcn.cdnleiting.top

x |= (1 << 3);
来源：http://mqq.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://byd.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zzi.dashuyun.cn

[S18] C：命令行参数
来源：http://dlo.vehdjk.com

int main(int argc, char **argv)
来源：http://ckb.aizwys.cn

[S19] C：快速排序
来源：http://jxs.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://eyt.hnqzz.top

[S20] C：二分查找
来源：http://ihe.smart0.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lki.nanxinkj.top

[S21] C：字符类别判断
来源：http://lzz.c1oappe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vxw.ywan-chungtsiang.top

[S22] C：字符串转数字
来源：http://mti.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://glb.hesvh.cn

[S23] C：随机数
来源：http://mrn.sysykeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://emw.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://wtn.zhoulong.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bvz.kuanghao11.cn

[S25] C：内存拷贝
来源：http://rtq.redwolf501.top

memcpy(dst, src, n);
来源：http://waj.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://tpb.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://mff.hfpthk.cn

[S27] C：定义常量
来源：http://ltw.havefunace.top

const double PI = 3.14159;
来源：http://sor.c1oappe.top

[S28] C：静态变量
来源：http://npo.kuanghao11.cn

static int counter = 0;
来源：http://ygy.svipenyu.cn

[S29] C：变参函数
来源：http://pdc.hywenlv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hkg.guowangkeji.top

[S30] C：头文件保护
来源：http://iwi.vehdjk.com

#ifndef X_H
来源：http://gzv.sxryk.cn

#define X_H
来源：http://syt.jqgufenzy.top

#endif
来源：http://tln.ppjwa.cn

[S31] C++：Hello World
来源：http://yum.tanke756.top

#include <iostream>
来源：http://bat.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://jjz.cdnleiting.top

[S32] C++：字符串
来源：http://src.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://gsd.hfpthk.cn

[S33] C++：vector 增删
来源：http://bsd.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tyf.cdnleiting.top

[S34] C++：遍历 vector
来源：http://axk.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://mkq.guannengcc.top

[S35] C++：map
来源：http://waq.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yzu.ivvv.top

[S36] C++：unordered_map
来源：http://vbq.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gic.quarkkingdee.top

[S37] C++：set
来源：http://rgs.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uza.hesvh.cn

[S38] C++：排序
来源：http://vzb.tianlin.xyz

std::sort(v.begin(), v.end());
来源：http://wms.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://sbq.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kny.ctjpmb.com

[S40] C++：查找元素
来源：http://nsd.xingfuxueyuan.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://khk.jlsjyb.cn

[S41] C++：类与构造函数
来源：http://bvo.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ykk.epnwcf.com

[S42] C++：继承与虚函数
来源：http://sib.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://tua.zhixingplan.top

[S43] C++：智能指针
来源：http://lln.hongshengwenyu.top

auto p = std::make_unique<int>(5);
来源：http://nzj.yfazqb.com

[S44] C++：引用传参
来源：http://fzk.iojbl.cn

void inc(int &x) { ++x; }
来源：http://xpw.daxiang520.top

[S45] C++：lambda
来源：http://gyx.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rrm.tarul.cn

[S46] C++：函数模板
来源：http://puh.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wao.quarkkingdee.top

[S47] C++：结构化绑定遍历
来源：http://npm.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hbg.sysykeji.top

[S48] C++：逐行读文件
来源：http://vgh.fanxiaobao.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://owi.zhengqikj.top

while (std::getline(in, line)) { }
来源：http://ika.yongpay.top

[S49] C++：写文件
来源：http://vag.yangfankeji.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://czf.daxiang520.top

[S50] C++：格式化数字
来源：http://dro.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://djs.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://wds.yongpay.top

static_cast<double>(a) / b
来源：http://akn.svipenyu.cn

[S52] C++：const 与 noexcept
来源：http://qif.fengsongda.top

int size() const noexcept { return n_; }
来源：http://htg.redwolf501.top

[S53] C++：移动语义
来源：http://xkj.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://xtq.gaohongyu789.top

[S54] C++：异常处理
来源：http://ixi.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iwk.gzhubu.top

[S55] C++：结构化绑定
来源：http://wvm.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zup.nwbrower.top

[S56] C++：optional
来源：http://mdp.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lbj.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://ppx.smart0.xyz

constexpr int N = 10;
来源：http://lkl.yfazqb.com

[S58] C++：命名空间
来源：http://aei.quarkkingdee.top

namespace ns { int f() { return 1; } }
来源：http://wgd.havefunace.top

[S59] C++：静态断言
来源：http://nma.hongshengwenyu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xpe.cashguo.top

[S60] C++：遍历并删除元素
来源：http://hgr.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hes.yongpay.top

================================================================================
来源：http://rgv.gotoacloud.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mmp.fzhhl.top

================================================================================
来源：http://gur.ehwqpu.com

[T01] Kotlin：Hello World
来源：http://ucp.yueranfly.top

println("Hello")
来源：http://tgs.ydjk.org.cn

[T02] Kotlin：变量
来源：http://dgk.nanxuanxn.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cwe.sysykeji.top

[T03] Kotlin：字符串模板
来源：http://eeo.gaohongyu789.top

"值: $b"
来源：http://euu.jyoumei.cn

[T04] Kotlin：空安全
来源：http://beq.zdqjudy.top

val n: String? = null;  n?.length
来源：http://rcl.jinghuilouyu.cn

[T05] Kotlin：when 表达式
来源：http://wqo.cdnleiting.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://isj.hcnkem.com

[T06] Kotlin：集合映射
来源：http://yjr.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://imv.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://mvt.jqgufenzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wfo.zycfv.cn

[T08] Kotlin：数据类
来源：http://qgw.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://bwy.yj202588.top

[T09] Kotlin：扩展函数
来源：http://fuf.gaohongyu789.top

fun String.exclaim() = this + "!"
来源：http://els.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://ike.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vhf.hammf.cn

[T11] Kotlin：协程
来源：http://iik.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fij.andypj.xyz

[T12] Kotlin：解构声明
来源：http://xqf.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://gab.shzxlz.cn


<!-- 参考信息 -->