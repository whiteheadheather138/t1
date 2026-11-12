代发 wailian999

case "$1" in
来源：http://eme.cdnleiting.top

start) echo "启动" ;;
来源：http://mtv.vehdjk.com

stop)  echo "停止" ;;
来源：http://kru.yangfankeji.com

*)     echo "未知命令" ;;
来源：http://qdr.nanxinkj.top

esac
来源：http://orn.pycfn.com

[R12] for 遍历文件
来源：http://uzj.aibaodan.cn

for f in *.txt; do echo "$f"; done
来源：http://dxi.ydzc1.top

[R13] for 计数循环
来源：http://wam.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://uqw.yfazqb.com

[R14] C 风格 for
来源：http://yrc.quarkkingdee.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bha.svipenyu.cn

[R15] while 逐行读文件
来源：http://cum.yanxiufei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dfo.hfpthk.cn

[R16] until 等待条件
来源：http://vpj.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dlm.uphjek.com

[R17] 数组定义与取值
来源：http://kje.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xtt.wangshuangyany.cn

[R18] 遍历数组
来源：http://ind.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cjr.yvedp.cn

[R19] 数组长度
来源：http://lty.jqgfzy.top

echo "${#arr[@]}"
来源：http://egi.jiagoushi.top

[R20] 关联数组（字典）
来源：http://irk.ywan-chungtsiang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fhx.yonumen.top

[R21] 字符串长度
来源：http://zwh.dianchejie.cn

echo "${#s}"
来源：http://xeq.ehwqpu.com

[R22] 截取子串
来源：http://yqg.316326.xyz

echo "${s:0:5}"
来源：http://hlq.bjfxy.top

[R23] 字符串替换
来源：http://kkr.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://euq.snrcjt.cn

[R24] 大小写转换
来源：http://kst.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://tze.gzhubu.top

[R25] 去后缀 / 去前缀
来源：http://ywt.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qjr.gzhubu.top

[R26] 命令替换
来源：http://bqv.yfazqb.com

now=$(date +%F); echo "$now"
来源：http://xto.meibo888.top

[R27] 算术展开
来源：http://usi.vqdsnc.cn

echo $((1 + 2 * 3))
来源：http://pzj.yj20258888.top

[R28] 浮点运算
来源：http://hdi.gogol.net.cn

echo "scale=2; 10/3" | bc
来源：http://fum.xziqi.cn

[R29] 定义函数
来源：http://smf.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://amp.jinyuanbaomall.cn

[R30] 函数返回状态码
来源：http://cfr.quarkkingdee.top

f() { return 0; }; f || echo "失败了"
来源：http://psg.sjlbkw.cn

[R31] 局部变量
来源：http://qgr.shzxlz.cn

f() { local x=1; echo "$x"; }
来源：http://nla.vqdsnc.cn

[R32] 参数个数校验
来源：http://ugo.jyoumei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://knw.ybcxt.top

[R33] 捕获错误并提示行号
来源：http://xut.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ayt.hcnkem.com

[R34] 退出时清理
来源：http://nmc.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xjy.cashguo.top

[R35] 后台执行并等待
来源：http://zxh.cdnleiting.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mye.yangfankeji.com

[R36] 并发执行多个任务
来源：http://yrg.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dsx.shangyingyoupin.top

[R37] 把输出赋给变量
来源：http://abx.52xcode.cn

files=$(ls -1)
来源：http://yoj.fzhhl.top

[R38] 管道串联
来源：http://dvj.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://vvk.chenzaomai.com

[R39] 重定向标准输出与错误
来源：http://vqa.hysaishi.cn

cmd > out.log 2>&1
来源：http://fsy.sufxvd.cn

[R40] 追加写日志
来源：http://chp.jlsjyb.cn

echo "log" >> out.log
来源：http://zhv.bbcook.cn

[R41] 丢弃输出
来源：http://xfw.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://zot.52xcode.cn

[R42] 输入重定向
来源：http://uew.jlsjyb.cn

wc -l < a.txt
来源：http://xup.tian-w.cn

[R43] 按名字查找文件
来源：http://jzh.havefunace.top

find . -name "*.log" -type f
来源：http://uze.hywenlv.cn

[R44] 按修改时间查找
来源：http://prn.52xcode.cn

find . -mtime -7 -type f
来源：http://jiq.pycfn.com

[R45] 批量删除
来源：http://ooi.mhx1999.top

find . -name "*.tmp" -delete
来源：http://fgx.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://umf.ydzc1.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bqu.jinqigfzy.top

[R47] sed 单行替换
来源：http://ijy.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://zhc.chenjidiqi.icu

[R48] awk 取指定列
来源：http://dhv.kuanghao11.cn

awk '{print $1, $3}' a.txt
来源：http://vec.52xcode.cn

[R49] awk 带条件
来源：http://skn.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mqo.kuanghao11.cn

[R50] awk 求和
来源：http://jsb.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xnz.gaohongyu789.top

[R51] 排序去重取前几
来源：http://pyu.hongshengwenyu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ige.fktsv.cn

[R52] 统计行数
来源：http://urw.zhixingplan.top

wc -l a.txt
来源：http://vvv.chenzaomai.com

[R53] 查看文件头与实时尾
来源：http://udq.yj20258888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://upg.fehbvm.com

[R54] 比较两个文件
来源：http://bft.guannengcc.top

diff a.txt b.txt
来源：http://mqh.yueranfly.top

[R55] 压缩与解压
来源：http://yhm.0kj1m.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://els.birdmap.top

[R56] 远程拷贝
来源：http://rqz.xingfuxueyuan.xyz

scp file user@host:/path/
来源：http://nva.jinghuilouyu.cn

[R57] 远程执行命令
来源：http://gwd.smart0.xyz

ssh user@host 'uptime'
来源：http://mxz.hysaishi.cn

[R58] 下载文件
来源：http://sar.ydjk.org.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qcw.yvedp.cn

[R59] 发 POST JSON
来源：http://azl.ppjwa.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xob.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://pai.jyoumei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vld.ydzc1.top

[R61] 磁盘占用
来源：http://nui.yangfankeji.com

df -h;  du -sh *
来源：http://zwn.zhengqikj.top

[R62] 找最占空间的文件
来源：http://pvp.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://vqr.9152youxi.cn

[R63] 内存与进程
来源：http://yqf.bbcook.cn

free -h;  ps aux | grep nginx
来源：http://bvp.xziqi.cn

[R64] 结束进程
来源：http://aek.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://rdn.wangdashe.top

[R65] 查看端口占用
来源：http://ypz.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qgv.uphjek.com

[R66] 定时任务
来源：http://ycd.gaohongyu789.top

crontab -e;  crontab -l
来源：http://yyf.cashguo.top

[R67] 生成随机十六进制串
来源：http://iil.zhijiandao.cn

openssl rand -hex 16
来源：http://tbb.havefunace.top

[R68] 计算文件校验值
来源：http://vew.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://odh.nwbrower.top

[R69] 生成随机密码
来源：http://rco.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://drv.tanke756.top

[R70] 时间戳与互转
来源：http://ahw.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://bgi.bjfxy.top

[R71] 日期格式化
来源：http://ovt.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mwr.cashguo.top

[R72] 等待端口就绪
来源：http://xiw.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ucv.zhongyouzk.top

[R73] 分割大日志
来源：http://kdt.jqgfzy.top

split -l 1000 big.log part_
来源：http://wgo.fktsv.cn

[R74] 批量重命名
来源：http://wry.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://llx.uphjek.com

[R75] 导出环境变量
来源：http://gex.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://mci.jianghu66.top

[R76] 使用临时文件
来源：http://lxt.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://syq.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://onb.tian-w.cn

read -rp "请输入: " ans
来源：http://slj.xinyue.icu

[R78] 交互式菜单
来源：http://nie.tian-w.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cdn.ybcxt.top

[R79] 解析命令行选项
来源：http://txz.jqgfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qme.ivvv.top

[R80] 查看脚本执行耗时
来源：http://ozv.hammf.cn

time ./run.sh
来源：http://osk.meibo888.top

================================================================================
来源：http://wdy.snrcjt.cn

S. C / C++ 专题
来源：http://hjf.aizwys.cn

================================================================================
来源：http://fwe.mhx1999.top

[S01] C：Hello World
来源：http://ihj.yuanzhike.top

#include <stdio.h>
来源：http://bjt.shanyushiyangtech.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xqb.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://dhk.daria6918.cn

int a = 10; printf("%d\n", a);
来源：http://suo.daria6918.cn

[S03] C：读入整数
来源：http://tkl.fehbvm.com

int x; scanf("%d", &x);
来源：http://yqu.yuanzhike.top

[S04] C：字符串复制
来源：http://zhf.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ytb.dashuyun.cn

[S05] C：字符串长度
来源：http://zkh.hongshengwenyu.top

strlen(s)
来源：http://btq.hongshengwenyu.top

[S06] C：字符串比较
来源：http://gdy.jqgufenzy.top

strcmp(a, b) == 0
来源：http://gjb.0kj1m.cn

[S07] C：数组遍历求和
来源：http://zgk.havefunace.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tis.zhixingplan.top

[S08] C：动态内存分配与释放
来源：http://lir.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hzo.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://cxp.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pai.shanyushiyangtech.top

[S10] C：指针与解引用
来源：http://mkn.yueranfly.top

int *p = &a;  *p = 5;
来源：http://hap.zhongyouzk.top

[S11] C：逐行读文件
来源：http://rwt.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://jmm.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lzt.yj20258.top

fclose(f);
来源：http://iox.c1oappe.top

[S12] C：写文件
来源：http://jep.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nzy.shzxlz.cn

[S13] C：宏定义
来源：http://eoh.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://afq.bbcook.cn

[S14] C：枚举
来源：http://zkw.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://vhi.andypj.xyz

[S15] C：类型转换
来源：http://upq.yanxiufei.cn

(double) a / b
来源：http://bca.sufxvd.cn

[S16] C：位操作置位
来源：http://vbh.yonumen.top

x |= (1 << 3);
来源：http://vyd.smart0.xyz

[S17] C：安全拼接字符串
来源：http://wyc.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mfr.nanxuanxn.top

[S18] C：命令行参数
来源：http://ajc.yonumen.top

int main(int argc, char **argv)
来源：http://ecm.nwbrower.top

[S19] C：快速排序
来源：http://srp.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://wzi.hammf.cn

[S20] C：二分查找
来源：http://gyq.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vbo.jqgufenzy.top

[S21] C：字符类别判断
来源：http://cnx.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qwt.epnwcf.com

[S22] C：字符串转数字
来源：http://tzl.redwolf501.top

atoi("42");  strtod("3.14", NULL);
来源：http://sgl.hesvh.cn

[S23] C：随机数
来源：http://fev.chenjidiqi.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://ghz.cucudq.cn

[S24] C：获取本地时间
来源：http://oes.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uuu.cucudq.cn

[S25] C：内存拷贝
来源：http://lsq.vehdjk.com

memcpy(dst, src, n);
来源：http://eor.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://lbb.chenlongwang.top

memset(a, 0, sizeof a);
来源：http://ffj.cashguo.top

[S27] C：定义常量
来源：http://htk.yj202588.top

const double PI = 3.14159;
来源：http://ybz.meibo888.top

[S28] C：静态变量
来源：http://euc.xziqi.cn

static int counter = 0;
来源：http://vtg.52xcode.cn

[S29] C：变参函数
来源：http://dmg.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ezl.gzhubu.top

[S30] C：头文件保护
来源：http://aui.tian-w.cn

#ifndef X_H
来源：http://qgc.hcnkem.com

#define X_H
来源：http://bvj.zhengqikj.top

#endif
来源：http://csy.aibaodan.cn

[S31] C++：Hello World
来源：http://dex.birdmap.top

#include <iostream>
来源：http://niw.xziqi.cn

int main() { std::cout << "Hello\n"; }
来源：http://ggw.hammf.cn

[S32] C++：字符串
来源：http://ckn.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://djx.bjfxy.top

[S33] C++：vector 增删
来源：http://hbt.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://spl.xuanzx.com

[S34] C++：遍历 vector
来源：http://lnw.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://rsi.gogol.net.cn

[S35] C++：map
来源：http://qdu.iojbl.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yht.hnqzz.top

[S36] C++：unordered_map
来源：http://byu.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ncc.redwolf501.top

[S37] C++：set
来源：http://idg.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://flo.zhongyouzk.top

[S38] C++：排序
来源：http://rgh.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://tbx.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://ysf.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vha.jinqigfzy.top

[S40] C++：查找元素
来源：http://cmc.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zgl.ppjwa.cn

[S41] C++：类与构造函数
来源：http://fpz.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ork.gogol.net.cn

[S42] C++：继承与虚函数
来源：http://qop.hongshengwenyu.top

class B : public Base { public: void f() override {} };
来源：http://kms.sjlbkw.cn

[S43] C++：智能指针
来源：http://wci.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://vdk.cdnleiting.top

[S44] C++：引用传参
来源：http://nsx.sxryk.cn

void inc(int &x) { ++x; }
来源：http://zld.epnwcf.com

[S45] C++：lambda
来源：http://vbw.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gid.chenzaomai.com

[S46] C++：函数模板
来源：http://wec.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oab.zhijiandao.cn

[S47] C++：结构化绑定遍历
来源：http://axp.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kbb.sxryk.cn

[S48] C++：逐行读文件
来源：http://lwu.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oqi.yuxming.cn

while (std::getline(in, line)) { }
来源：http://gzk.tianlin.xyz

[S49] C++：写文件
来源：http://cmd.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iwo.nanxuanxn.top

[S50] C++：格式化数字
来源：http://tcq.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dmx.hywenlv.cn

[S51] C++：显式类型转换
来源：http://shm.yongpay.top

static_cast<double>(a) / b
来源：http://uki.ppjwa.cn

[S52] C++：const 与 noexcept
来源：http://ucj.c1oappe.top

int size() const noexcept { return n_; }
来源：http://ueo.xziqi.cn

[S53] C++：移动语义
来源：http://tib.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://wsh.shuidangran.top

[S54] C++：异常处理
来源：http://wfa.birdmap.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nhj.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://axe.shanyushiyangtech.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dkw.nanxinkj.top

[S56] C++：optional
来源：http://ndr.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nvy.gotoacloud.top

[S57] C++：编译期常量
来源：http://raa.zhixingplan.top

constexpr int N = 10;
来源：http://mwd.xziqi.cn

[S58] C++：命名空间
来源：http://eru.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://asb.xylfe.cn

[S59] C++：静态断言
来源：http://wtc.daxiang520.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://krf.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://pnv.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yhq.snrcjt.cn

================================================================================
来源：http://wgc.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vxz.havefunace.top

================================================================================
来源：http://dwg.ybcxt.top

[T01] Kotlin：Hello World
来源：http://iyr.smart0.xyz

println("Hello")
来源：http://qpe.uphjek.com

[T02] Kotlin：变量
来源：http://qrb.daria6918.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oey.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://kxq.jqgfzy.top

"值: $b"
来源：http://cbf.pycfn.com

[T04] Kotlin：空安全
来源：http://xxg.hammf.cn

val n: String? = null;  n?.length
来源：http://trr.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://hfq.vehdjk.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ymx.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://afu.nwbrower.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tcd.hnqzz.top

[T07] Kotlin：集合过滤
来源：http://yxo.wangdashe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nrn.meibo888.top

[T08] Kotlin：数据类
来源：http://ler.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://tab.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://wix.jiagoushi.top

fun String.exclaim() = this + "!"
来源：http://miu.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://lkq.52xcode.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mly.jqgfzy.top

[T11] Kotlin：协程
来源：http://mqn.yangfankeji.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://icw.zdbjq.cn

[T12] Kotlin：解构声明
来源：http://phi.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://ihd.hesvh.cn


<!-- 参考信息 -->