代发 wailian999

esac
来源：http://yqb.cdnleiting.top

[R12] for 遍历文件
来源：http://wmj.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://imh.yuxming.cn

[R13] for 计数循环
来源：http://xkd.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://iwv.tianlin.xyz

[R14] C 风格 for
来源：http://olc.ctjpmb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kfr.tanke756.top

[R15] while 逐行读文件
来源：http://ram.nanxuanxn.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pzi.yanxiufei.cn

[R16] until 等待条件
来源：http://hvk.cdnleiting.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fvd.0kj1m.cn

[R17] 数组定义与取值
来源：http://vch.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nkw.bjfxy.top

[R18] 遍历数组
来源：http://mwi.tarul.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://phv.birdmap.top

[R19] 数组长度
来源：http://lad.wangdashe.top

echo "${#arr[@]}"
来源：http://lzg.jqgufenzy.top

[R20] 关联数组（字典）
来源：http://yhz.zhiwuduotai.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jyp.ywan-chungtsiang.top

[R21] 字符串长度
来源：http://kfb.jinqigufen.top

echo "${#s}"
来源：http://qvu.svipenyu.cn

[R22] 截取子串
来源：http://dap.jinghuilouyu.cn

echo "${s:0:5}"
来源：http://vbb.smart0.xyz

[R23] 字符串替换
来源：http://gwc.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fjk.xziqi.cn

[R24] 大小写转换
来源：http://esb.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://dkv.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://qyp.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vhf.yfazqb.com

[R26] 命令替换
来源：http://amv.hongshengwenyu.top

now=$(date +%F); echo "$now"
来源：http://nth.zycfv.cn

[R27] 算术展开
来源：http://tbn.yj202588.top

echo $((1 + 2 * 3))
来源：http://axt.gzhubu.top

[R28] 浮点运算
来源：http://vsd.yfazqb.com

echo "scale=2; 10/3" | bc
来源：http://ymo.xziqi.cn

[R29] 定义函数
来源：http://gwk.meibo888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mdg.52xcode.cn

[R30] 函数返回状态码
来源：http://cmf.jinyuanbaomall.cn

f() { return 0; }; f || echo "失败了"
来源：http://hdc.iojbl.cn

[R31] 局部变量
来源：http://kod.feifeiyinyue.top

f() { local x=1; echo "$x"; }
来源：http://xrg.jqgufenzy.top

[R32] 参数个数校验
来源：http://gkp.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bfv.xuanzx.com

[R33] 捕获错误并提示行号
来源：http://hwf.epnwcf.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nbl.jianghu66.top

[R34] 退出时清理
来源：http://zah.gzhubu.top

trap 'rm -f "$tmp"' EXIT
来源：http://knd.ivvv.top

[R35] 后台执行并等待
来源：http://ohd.zhijiandao.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rqk.zhaomingkeji.xyz

[R36] 并发执行多个任务
来源：http://inb.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lsy.xylfe.cn

[R37] 把输出赋给变量
来源：http://suu.ybcxt.top

files=$(ls -1)
来源：http://guc.shuidangran.top

[R38] 管道串联
来源：http://pon.tarul.cn

cat a.txt | grep -i error | wc -l
来源：http://tvk.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://dyv.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://etl.cheryme.top

[R40] 追加写日志
来源：http://vcv.gotoacloud.top

echo "log" >> out.log
来源：http://mkk.nanxinkj.top

[R41] 丢弃输出
来源：http://wbk.birdmap.top

cmd >/dev/null 2>&1
来源：http://axc.0kj1m.cn

[R42] 输入重定向
来源：http://qjt.hnxiangtu.top

wc -l < a.txt
来源：http://cwt.yj202588.top

[R43] 按名字查找文件
来源：http://wra.shanyushiyangkeji.top

find . -name "*.log" -type f
来源：http://hrz.jiagoushi.top

[R44] 按修改时间查找
来源：http://gxv.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://ust.hammf.cn

[R45] 批量删除
来源：http://vmt.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://fhe.gaohongyu789.top

[R46] 递归替换文件内容
来源：http://bti.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://osx.yvedp.cn

[R47] sed 单行替换
来源：http://why.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://quw.hcnkem.com

[R48] awk 取指定列
来源：http://gzw.gotoacloud.top

awk '{print $1, $3}' a.txt
来源：http://bod.yj20258888.top

[R49] awk 带条件
来源：http://gcy.gaohongyu789.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qpe.yj20258.top

[R50] awk 求和
来源：http://egx.dashuyun.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cwr.iojbl.cn

[R51] 排序去重取前几
来源：http://tlq.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dsa.dashuyun.cn

[R52] 统计行数
来源：http://flk.c1oappe.top

wc -l a.txt
来源：http://xua.havefunace.top

[R53] 查看文件头与实时尾
来源：http://mwi.dashuyun.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fia.xinyue.icu

[R54] 比较两个文件
来源：http://qps.hnqzz.top

diff a.txt b.txt
来源：http://tgu.jqgfzy.top

[R55] 压缩与解压
来源：http://mln.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lux.pycfn.com

[R56] 远程拷贝
来源：http://cna.zycfv.cn

scp file user@host:/path/
来源：http://sfe.xinyue.icu

[R57] 远程执行命令
来源：http://ofn.hnxiangtu.top

ssh user@host 'uptime'
来源：http://lcz.bjfxy.top

[R58] 下载文件
来源：http://gpx.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gvt.birdmap.top

[R59] 发 POST JSON
来源：http://eyn.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://idv.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://wvj.guannengcc.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oeu.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://bic.chenlongwang.top

df -h;  du -sh *
来源：http://tvk.ydzc1.top

[R62] 找最占空间的文件
来源：http://tub.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://gco.iojbl.cn

[R63] 内存与进程
来源：http://bys.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://kcf.cdnleiting.top

[R64] 结束进程
来源：http://zaw.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://hav.uphjek.com

[R65] 查看端口占用
来源：http://bpq.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://txg.aizwys.cn

[R66] 定时任务
来源：http://zak.chenjidiqi.icu

crontab -e;  crontab -l
来源：http://koa.tian-w.cn

[R67] 生成随机十六进制串
来源：http://nah.fanxiaobao.xyz

openssl rand -hex 16
来源：http://fsk.tian-w.cn

[R68] 计算文件校验值
来源：http://vns.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://aff.hnxiangtu.top

[R69] 生成随机密码
来源：http://pve.yonumen.top

head -c 16 /dev/urandom | base64
来源：http://xcs.zycfv.cn

[R70] 时间戳与互转
来源：http://lgs.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://ymz.gaohongyu789.top

[R71] 日期格式化
来源：http://ekk.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xub.meibo888.top

[R72] 等待端口就绪
来源：http://uvp.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tpq.sxryk.cn

[R73] 分割大日志
来源：http://xdm.svipenyu.cn

split -l 1000 big.log part_
来源：http://dpz.c1oappe.top

[R74] 批量重命名
来源：http://goh.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fub.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://pqb.guannengcc.top

export PATH="$HOME/bin:$PATH"
来源：http://ttf.fengsongda.top

[R76] 使用临时文件
来源：http://mcm.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ycv.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://gda.yuxming.cn

read -rp "请输入: " ans
来源：http://bei.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://tlp.zhongyouzk.top

select opt in a b c; do echo "$opt"; break; done
来源：http://owa.sweek.top

[R79] 解析命令行选项
来源：http://cuj.epnwcf.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uew.birdmap.top

[R80] 查看脚本执行耗时
来源：http://byi.svipenyu.cn

time ./run.sh
来源：http://ctk.ydjk.org.cn

================================================================================
来源：http://rlq.zhongyouzk.top

S. C / C++ 专题
来源：http://qwt.fehbvm.com

================================================================================
来源：http://rda.hesvh.cn

[S01] C：Hello World
来源：http://lyy.sufxvd.cn

#include <stdio.h>
来源：http://lgp.jlsjyb.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gjk.birdmap.top

[S02] C：变量与格式化输出
来源：http://ahw.mhx1999.top

int a = 10; printf("%d\n", a);
来源：http://lck.ydjk.org.cn

[S03] C：读入整数
来源：http://nzq.ehwqpu.com

int x; scanf("%d", &x);
来源：http://owy.vehdjk.com

[S04] C：字符串复制
来源：http://ndg.jianghu66.top

char dst[32]; strcpy(dst, "hi");
来源：http://urq.birdmap.top

[S05] C：字符串长度
来源：http://asa.zycfv.cn

strlen(s)
来源：http://yya.cucudq.cn

[S06] C：字符串比较
来源：http://bal.wangdashe.top

strcmp(a, b) == 0
来源：http://dfi.tian-w.cn

[S07] C：数组遍历求和
来源：http://lkp.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oyv.jqgfzy.top

[S08] C：动态内存分配与释放
来源：http://evx.zycfv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://duf.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://hry.smart0.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yvx.fktsv.cn

[S10] C：指针与解引用
来源：http://zqt.sjlbkw.cn

int *p = &a;  *p = 5;
来源：http://edo.guowangkeji.top

[S11] C：逐行读文件
来源：http://bun.uphjek.com

FILE *f = fopen("a.txt", "r");
来源：http://mas.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mui.gogol.net.cn

fclose(f);
来源：http://ffy.wangshuangyany.cn

[S12] C：写文件
来源：http://kma.xuetiantiany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://knx.sufxvd.cn

[S13] C：宏定义
来源：http://vdb.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lsx.xuetiantiany.cn

[S14] C：枚举
来源：http://lyd.tian-w.cn

enum Color { RED, GREEN, BLUE };
来源：http://prc.shzxlz.cn

[S15] C：类型转换
来源：http://mer.dianchejie.cn

(double) a / b
来源：http://yne.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://dem.dianchejie.cn

x |= (1 << 3);
来源：http://rgb.hywenlv.cn

[S17] C：安全拼接字符串
来源：http://noj.aibaodan.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://thl.hnqzz.top

[S18] C：命令行参数
来源：http://eii.zhengqikj.top

int main(int argc, char **argv)
来源：http://jnm.zhoulong.xyz

[S19] C：快速排序
来源：http://ach.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://hen.feifeiyinyue.top

[S20] C：二分查找
来源：http://bmp.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://exw.havefunace.top

[S21] C：字符类别判断
来源：http://mko.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kos.0kj1m.cn

[S22] C：字符串转数字
来源：http://zso.kuanghao11.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iti.yangfankeji.com

[S23] C：随机数
来源：http://oip.jinqigufen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dwn.smart0.xyz

[S24] C：获取本地时间
来源：http://jno.wangshuangyany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bef.xziqi.cn

[S25] C：内存拷贝
来源：http://sao.andypj.xyz

memcpy(dst, src, n);
来源：http://msp.gotoacloud.top

[S26] C：内存清零
来源：http://fbe.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://dxj.havefunace.top

[S27] C：定义常量
来源：http://ism.guannengcc.top

const double PI = 3.14159;
来源：http://qlr.ydzc1.top

[S28] C：静态变量
来源：http://chj.nanxinkj.top

static int counter = 0;
来源：http://rfb.xinyue.icu

[S29] C：变参函数
来源：http://udw.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oqf.fktsv.cn

[S30] C：头文件保护
来源：http://eab.yuanzhike.top

#ifndef X_H
来源：http://iut.zhaomingkeji.xyz

#define X_H
来源：http://pga.yj20258.top

#endif
来源：http://tot.vqdsnc.cn

[S31] C++：Hello World
来源：http://luj.hnqzz.top

#include <iostream>
来源：http://anp.fzhhl.top

int main() { std::cout << "Hello\n"; }
来源：http://mok.zdbjq.cn

[S32] C++：字符串
来源：http://flf.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://rvf.guannengcc.top

[S33] C++：vector 增删
来源：http://ocp.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jwm.tianlin.xyz

[S34] C++：遍历 vector
来源：http://zuv.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://dhb.yvedp.cn

[S35] C++：map
来源：http://jti.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nwe.kuanghao11.cn

[S36] C++：unordered_map
来源：http://xzy.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cxy.daria6918.cn

[S37] C++：set
来源：http://ofe.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lzt.meibo888.top

[S38] C++：排序
来源：http://wka.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://kbh.havefunace.top

[S39] C++：自定义比较器排序
来源：http://tdj.zhoulong.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aul.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://bwn.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jdv.cdnleiting.top

[S41] C++：类与构造函数
来源：http://vvt.yfazqb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rvt.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://pjh.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://yag.zycfv.cn

[S43] C++：智能指针
来源：http://vuh.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://qdl.ydzc1.top

[S44] C++：引用传参
来源：http://sus.cashguo.top

void inc(int &x) { ++x; }
来源：http://tju.xziqi.cn

[S45] C++：lambda
来源：http://gla.0kj1m.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fwf.meibo888.top

[S46] C++：函数模板
来源：http://jot.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mhl.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://svf.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://olt.fengsongda.top

[S48] C++：逐行读文件
来源：http://wuz.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://vxf.nanxuanxn.top

while (std::getline(in, line)) { }
来源：http://odw.epnwcf.com

[S49] C++：写文件
来源：http://fbf.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uzj.xinyue.icu

[S50] C++：格式化数字
来源：http://gdz.nanxuanxn.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pnl.snrcjt.cn

[S51] C++：显式类型转换
来源：http://htm.guowangkeji.top

static_cast<double>(a) / b
来源：http://smr.hfpthk.cn

[S52] C++：const 与 noexcept
来源：http://oql.yongpay.top

int size() const noexcept { return n_; }
来源：http://mnr.tianlin.xyz

[S53] C++：移动语义
来源：http://kul.tarul.cn

std::vector<int> w = std::move(v);
来源：http://tks.hfpthk.cn

[S54] C++：异常处理
来源：http://ddu.epnwcf.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gzk.cqqwz.cn

[S55] C++：结构化绑定
来源：http://yar.sysykeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ynb.kuanghao11.cn

[S56] C++：optional
来源：http://rjj.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jdb.gotoacloud.top

[S57] C++：编译期常量
来源：http://dps.xziqi.cn

constexpr int N = 10;
来源：http://uam.tanke756.top

[S58] C++：命名空间
来源：http://ftv.uphjek.com

namespace ns { int f() { return 1; } }
来源：http://pen.ydzc1.top

[S59] C++：静态断言
来源：http://pso.quarkkingdee.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gla.shzxlz.cn

[S60] C++：遍历并删除元素
来源：http://jkm.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oyd.tian-w.cn

================================================================================
来源：http://glj.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xga.dashuyun.cn

================================================================================
来源：http://qwe.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://iao.yvedp.cn

println("Hello")
来源：http://mxm.sweek.top

[T02] Kotlin：变量
来源：http://hhd.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qfc.meibo888.top

[T03] Kotlin：字符串模板
来源：http://paa.0kj1m.cn

"值: $b"
来源：http://pvc.zdbjq.cn

[T04] Kotlin：空安全
来源：http://qpk.ydzc1.top

val n: String? = null;  n?.length
来源：http://emg.cheryme.top

[T05] Kotlin：when 表达式
来源：http://sfq.yj20258888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ofa.fzhhl.top

[T06] Kotlin：集合映射
来源：http://wue.yueranfly.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zpz.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://bss.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eob.andypj.xyz

[T08] Kotlin：数据类
来源：http://mwi.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://hod.hongshengwenyu.top

[T09] Kotlin：扩展函数
来源：http://cnt.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://trr.svipenyu.cn

[T10] Kotlin：默认参数
来源：http://oum.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://odf.aibaodan.cn

[T11] Kotlin：协程
来源：http://nvw.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mav.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://szr.zhoulong.xyz

val (a, b) = Pair(1, 2)
来源：http://wxr.jinqigufen.top

[T13] Kotlin：只读 Map
来源：http://gvd.daxiang520.top

val m = mapOf("a" to 1)
来源：http://fwj.gaohongyu789.top

[T14] Kotlin：循环
来源：http://ild.fehbvm.com

for (i in 1..10) println(i)
来源：http://nli.316326.xyz


<!-- 参考信息 -->