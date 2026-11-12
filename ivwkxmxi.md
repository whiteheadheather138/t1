代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ldw.zhiwuduotai.top

[R16] until 等待条件
来源：http://rmu.snrcjt.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nfg.hysaishi.cn

[R17] 数组定义与取值
来源：http://aam.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://bqi.guannengcc.top

[R18] 遍历数组
来源：http://vxj.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ncq.yj202588.top

[R19] 数组长度
来源：http://frp.havefunace.top

echo "${#arr[@]}"
来源：http://vli.jqgufenzy.top

[R20] 关联数组（字典）
来源：http://jdb.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eqz.yj20258888.top

[R21] 字符串长度
来源：http://tju.tian-w.cn

echo "${#s}"
来源：http://pwr.zhixingplan.top

[R22] 截取子串
来源：http://exk.tarul.cn

echo "${s:0:5}"
来源：http://scb.316326.xyz

[R23] 字符串替换
来源：http://xna.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qbt.iojbl.cn

[R24] 大小写转换
来源：http://lxz.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uij.haohaochexian.top

[R25] 去后缀 / 去前缀
来源：http://fbp.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://jkz.hcnkem.com

[R26] 命令替换
来源：http://ngp.jinghuilouyu.cn

now=$(date +%F); echo "$now"
来源：http://zsj.zycfv.cn

[R27] 算术展开
来源：http://hvk.ivvv.top

echo $((1 + 2 * 3))
来源：http://lyo.mhx1999.top

[R28] 浮点运算
来源：http://bet.xingfuxueyuan.xyz

echo "scale=2; 10/3" | bc
来源：http://vuv.yuanzhike.top

[R29] 定义函数
来源：http://hjf.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eal.ppjwa.cn

[R30] 函数返回状态码
来源：http://guw.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://rso.smart0.xyz

[R31] 局部变量
来源：http://xah.xylfe.cn

f() { local x=1; echo "$x"; }
来源：http://upp.hfpthk.cn

[R32] 参数个数校验
来源：http://wne.ppjwa.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://god.dashuyun.cn

[R33] 捕获错误并提示行号
来源：http://aay.kuanghao11.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pru.yj20258.top

[R34] 退出时清理
来源：http://vwp.yvedp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kwm.zhixingplan.top

[R35] 后台执行并等待
来源：http://sgv.dianchejie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ooe.fktsv.cn

[R36] 并发执行多个任务
来源：http://gpx.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ktl.zhaomingkeji.xyz

[R37] 把输出赋给变量
来源：http://xrh.ydzc1.top

files=$(ls -1)
来源：http://ugu.haohaochexian.top

[R38] 管道串联
来源：http://bjz.yongpay.top

cat a.txt | grep -i error | wc -l
来源：http://tos.cqqwz.cn

[R39] 重定向标准输出与错误
来源：http://arv.cucudq.cn

cmd > out.log 2>&1
来源：http://cah.xylfe.cn

[R40] 追加写日志
来源：http://lmo.jqgfzy.top

echo "log" >> out.log
来源：http://qlc.bbcook.cn

[R41] 丢弃输出
来源：http://wfz.0kj1m.cn

cmd >/dev/null 2>&1
来源：http://ulv.fktsv.cn

[R42] 输入重定向
来源：http://pex.hywenlv.cn

wc -l < a.txt
来源：http://oje.aizwys.cn

[R43] 按名字查找文件
来源：http://kky.yfazqb.com

find . -name "*.log" -type f
来源：http://ulg.jiagoushi.top

[R44] 按修改时间查找
来源：http://tow.nanxuanxn.top

find . -mtime -7 -type f
来源：http://cgw.hnqzz.top

[R45] 批量删除
来源：http://krw.jinyuanbaomall.cn

find . -name "*.tmp" -delete
来源：http://mjj.epnwcf.com

[R46] 递归替换文件内容
来源：http://zcm.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rtx.jqgfzy.top

[R47] sed 单行替换
来源：http://dhz.yvedp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://aju.dianchejie.cn

[R48] awk 取指定列
来源：http://igx.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://sch.quarkkingdee.top

[R49] awk 带条件
来源：http://ydq.c1oappe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tcr.havefunace.top

[R50] awk 求和
来源：http://ewz.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://snn.9152youxi.cn

[R51] 排序去重取前几
来源：http://ehd.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pkx.0kj1m.cn

[R52] 统计行数
来源：http://rrb.sysykeji.top

wc -l a.txt
来源：http://sdk.jyoumei.cn

[R53] 查看文件头与实时尾
来源：http://lwo.zhaomingkeji.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ycq.sjlbkw.cn

[R54] 比较两个文件
来源：http://mar.jqgufenzy.top

diff a.txt b.txt
来源：http://sem.daria6918.cn

[R55] 压缩与解压
来源：http://rqj.dianchejie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gsp.meibo888.top

[R56] 远程拷贝
来源：http://ksp.cheryme.top

scp file user@host:/path/
来源：http://ylx.uphjek.com

[R57] 远程执行命令
来源：http://myp.tian-w.cn

ssh user@host 'uptime'
来源：http://xzq.feifeiyinyue.top

[R58] 下载文件
来源：http://hyd.aizwys.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://odk.meibo888.top

[R59] 发 POST JSON
来源：http://beh.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://boy.9152youxi.cn

[R60] 只看 HTTP 状态码
来源：http://yov.xuetiantiany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qpn.hnqzz.top

[R61] 磁盘占用
来源：http://aub.hnxiangtu.top

df -h;  du -sh *
来源：http://wrf.zhixingplan.top

[R62] 找最占空间的文件
来源：http://jvn.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://hdu.cheryme.top

[R63] 内存与进程
来源：http://zjz.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://kil.chenlongwang.top

[R64] 结束进程
来源：http://vut.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://lxi.hnqzz.top

[R65] 查看端口占用
来源：http://eia.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tmc.birdmap.top

[R66] 定时任务
来源：http://unf.guannengcc.top

crontab -e;  crontab -l
来源：http://eqg.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://hfc.jinghuilouyu.cn

openssl rand -hex 16
来源：http://gkv.meibo888.top

[R68] 计算文件校验值
来源：http://xom.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://tak.tian-w.cn

[R69] 生成随机密码
来源：http://dwz.andypj.xyz

head -c 16 /dev/urandom | base64
来源：http://rqe.shangyingyoupin.top

[R70] 时间戳与互转
来源：http://xfb.yj202588.top

date +%s;  date -d @1700000000
来源：http://qyo.vehdjk.com

[R71] 日期格式化
来源：http://haq.bbcook.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kwj.cheryme.top

[R72] 等待端口就绪
来源：http://ydu.bbcook.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nxw.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://dlc.epnwcf.com

split -l 1000 big.log part_
来源：http://xem.jqgufenzy.top

[R74] 批量重命名
来源：http://ofa.zdqjudy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rue.jiagoushi.top

[R75] 导出环境变量
来源：http://xyh.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://eyh.kuanghao11.cn

[R76] 使用临时文件
来源：http://bsl.316326.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xpe.sxryk.cn

[R77] 读取用户输入
来源：http://zoe.shanyushiyangkeji.top

read -rp "请输入: " ans
来源：http://vjr.bjfxy.top

[R78] 交互式菜单
来源：http://ynl.shanyushiyangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xfk.andypj.xyz

[R79] 解析命令行选项
来源：http://ihm.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yvl.chenzaomai.com

[R80] 查看脚本执行耗时
来源：http://oao.aibaodan.cn

time ./run.sh
来源：http://mng.gogol.net.cn

================================================================================
来源：http://agb.yj20258888.top

S. C / C++ 专题
来源：http://nix.ctjpmb.com

================================================================================
来源：http://xwk.epnwcf.com

[S01] C：Hello World
来源：http://hua.yuanzhike.top

#include <stdio.h>
来源：http://uqt.daxiang520.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kde.hesvh.cn

[S02] C：变量与格式化输出
来源：http://xle.svipenyu.cn

int a = 10; printf("%d\n", a);
来源：http://jvj.hnqzz.top

[S03] C：读入整数
来源：http://amv.chenjidiqi.icu

int x; scanf("%d", &x);
来源：http://qes.yueranfly.top

[S04] C：字符串复制
来源：http://mtj.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://tba.zdqjudy.top

[S05] C：字符串长度
来源：http://zly.yangfankeji.com

strlen(s)
来源：http://fhw.vehdjk.com

[S06] C：字符串比较
来源：http://hdb.hnxiangtu.top

strcmp(a, b) == 0
来源：http://xil.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://fiz.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jxe.hongshengwenyu.top

[S08] C：动态内存分配与释放
来源：http://npp.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aql.aibaodan.cn

[S09] C：结构体定义与初始化
来源：http://kcp.yonumen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uny.xuanzx.com

[S10] C：指针与解引用
来源：http://ejj.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://aex.jqgufenzy.top

[S11] C：逐行读文件
来源：http://brp.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://klc.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qbv.ppjwa.cn

fclose(f);
来源：http://zrj.c1oappe.top

[S12] C：写文件
来源：http://xus.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qot.yueranfly.top

[S13] C：宏定义
来源：http://lxy.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hxs.jlsjyb.cn

[S14] C：枚举
来源：http://yry.pycfn.com

enum Color { RED, GREEN, BLUE };
来源：http://fjk.jiagoushi.top

[S15] C：类型转换
来源：http://hnu.ybcxt.top

(double) a / b
来源：http://vgi.xziqi.cn

[S16] C：位操作置位
来源：http://ctx.pycfn.com

x |= (1 << 3);
来源：http://pym.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://dyc.yfazqb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pxw.yj20258.top

[S18] C：命令行参数
来源：http://uqk.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://yjd.xuanzx.com

[S19] C：快速排序
来源：http://uwz.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://qhm.meibo888.top

[S20] C：二分查找
来源：http://nry.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gkq.zdqjudy.top

[S21] C：字符类别判断
来源：http://rxk.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gbl.xuanzx.com

[S22] C：字符串转数字
来源：http://kzn.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://uei.mhx1999.top

[S23] C：随机数
来源：http://sjd.andypj.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://psa.zdqjudy.top

[S24] C：获取本地时间
来源：http://fjk.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://apa.xinyue.icu

[S25] C：内存拷贝
来源：http://uic.zhoulong.xyz

memcpy(dst, src, n);
来源：http://rjx.nanxinkj.top

[S26] C：内存清零
来源：http://wvl.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://bee.redwolf501.top

[S27] C：定义常量
来源：http://oxk.hnqzz.top

const double PI = 3.14159;
来源：http://lbr.wangshuangyany.cn

[S28] C：静态变量
来源：http://lxm.cqqwz.cn

static int counter = 0;
来源：http://rur.snrcjt.cn

[S29] C：变参函数
来源：http://ble.cheryme.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://prp.cashguo.top

[S30] C：头文件保护
来源：http://dvv.52xcode.cn

#ifndef X_H
来源：http://eay.daria6918.cn

#define X_H
来源：http://pde.cdnleiting.top

#endif
来源：http://dxh.hcnkem.com

[S31] C++：Hello World
来源：http://thl.yueranfly.top

#include <iostream>
来源：http://pvd.zhengqikj.top

int main() { std::cout << "Hello\n"; }
来源：http://quh.xuanzx.com

[S32] C++：字符串
来源：http://bfv.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://fyx.yonumen.top

[S33] C++：vector 增删
来源：http://bgj.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mfm.316326.xyz

[S34] C++：遍历 vector
来源：http://okp.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://quq.sysykeji.top

[S35] C++：map
来源：http://via.gogol.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://otg.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://vva.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yzn.andypj.xyz

[S37] C++：set
来源：http://dbn.nanxinkj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kxd.jinghuilouyu.cn

[S38] C++：排序
来源：http://hoq.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://ubj.ehwqpu.com

[S39] C++：自定义比较器排序
来源：http://dry.bjfxy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rrs.andypj.xyz

[S40] C++：查找元素
来源：http://vyu.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sfy.xingfuxueyuan.xyz

[S41] C++：类与构造函数
来源：http://zis.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ska.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://kkg.epnwcf.com

class B : public Base { public: void f() override {} };
来源：http://aei.jinqigfzy.top

[S43] C++：智能指针
来源：http://ufg.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://gjh.tianlin.xyz

[S44] C++：引用传参
来源：http://oxc.fktsv.cn

void inc(int &x) { ++x; }
来源：http://kmd.52xcode.cn

[S45] C++：lambda
来源：http://iyc.cashguo.top

auto add = [](int a, int b) { return a + b; };
来源：http://lqp.yangfankeji.com

[S46] C++：函数模板
来源：http://trg.yj20258.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ins.sweek.top

[S47] C++：结构化绑定遍历
来源：http://two.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rxs.cucudq.cn

[S48] C++：逐行读文件
来源：http://law.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yii.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://rmi.9152youxi.cn

[S49] C++：写文件
来源：http://cgb.guowangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cat.jiagoushi.top

[S50] C++：格式化数字
来源：http://dta.pycfn.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pzf.hcnkem.com

[S51] C++：显式类型转换
来源：http://kdz.sufxvd.cn

static_cast<double>(a) / b
来源：http://rkr.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://ast.xuanzx.com

int size() const noexcept { return n_; }
来源：http://llb.guannengcc.top

[S53] C++：移动语义
来源：http://uta.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://csl.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://efp.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ive.zdqjudy.top

[S55] C++：结构化绑定
来源：http://mvs.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://ggg.hcnkem.com

[S56] C++：optional
来源：http://lqt.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dtt.nanxuanxn.top

[S57] C++：编译期常量
来源：http://ipj.shanyushiyangkeji.top

constexpr int N = 10;
来源：http://hbq.yongpay.top

[S58] C++：命名空间
来源：http://glr.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://hxd.zycfv.cn

[S59] C++：静态断言
来源：http://krq.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ghw.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://ziz.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bna.pengpengdd.cyou

================================================================================
来源：http://eyq.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bug.hesvh.cn

================================================================================
来源：http://wsg.redwolf501.top

[T01] Kotlin：Hello World
来源：http://whu.gzhubu.top

println("Hello")
来源：http://qom.c1oappe.top

[T02] Kotlin：变量
来源：http://oqz.hywenlv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://esk.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://ldj.shanyushiyangkeji.top

"值: $b"
来源：http://gyt.xziqi.cn

[T04] Kotlin：空安全
来源：http://eln.hnqzz.top

val n: String? = null;  n?.length
来源：http://pbk.uphjek.com

[T05] Kotlin：when 表达式
来源：http://qzj.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cpj.smart0.xyz

[T06] Kotlin：集合映射
来源：http://abf.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uvv.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://xcz.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ept.cqqwz.cn

[T08] Kotlin：数据类
来源：http://ssw.pycfn.com

data class User(val name: String, val age: Int)
来源：http://mzn.gogol.net.cn

[T09] Kotlin：扩展函数
来源：http://vuu.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://may.uphjek.com

[T10] Kotlin：默认参数
来源：http://jpe.fehbvm.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ryg.sufxvd.cn

[T11] Kotlin：协程
来源：http://dpf.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xea.cucudq.cn

[T12] Kotlin：解构声明
来源：http://msu.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://sai.xuanzx.com

[T13] Kotlin：只读 Map
来源：http://mce.gotoacloud.top

val m = mapOf("a" to 1)
来源：http://vwr.kuanghao11.cn

[T14] Kotlin：循环
来源：http://gjo.yonumen.top

for (i in 1..10) println(i)
来源：http://juj.xuetiantiany.cn

[T15] Kotlin：接口
来源：http://ulx.jinyuanbaomall.cn

interface Shape { fun area(): Double }
来源：http://kqg.yuxming.cn

[T16] Swift：Hello World
来源：http://lls.daxiang520.top

print("Hello")
来源：http://afi.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://hhg.guannengcc.top

var a = 1;  let b = 2
来源：http://xao.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://vnx.tian-w.cn

"值: \(b)"
来源：http://uwc.sxryk.cn


<!-- 参考信息 -->