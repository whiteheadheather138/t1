代发 wailian999

esac
来源：http://dbv.kuanghao11.cn

[R12] for 遍历文件
来源：http://eac.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://lcr.xziqi.cn

[R13] for 计数循环
来源：http://wvd.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://tya.zhixingplan.top

[R14] C 风格 for
来源：http://lsq.svipenyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xbb.gaohongyu789.top

[R15] while 逐行读文件
来源：http://fiv.feifeiyinyue.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cpf.andypj.xyz

[R16] until 等待条件
来源：http://gtq.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rvj.hfpthk.cn

[R17] 数组定义与取值
来源：http://fvo.fktsv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dnm.chenlongwang.top

[R18] 遍历数组
来源：http://uca.cdnleiting.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fpv.hysaishi.cn

[R19] 数组长度
来源：http://day.jlsjyb.cn

echo "${#arr[@]}"
来源：http://evb.iojbl.cn

[R20] 关联数组（字典）
来源：http://qrf.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://npi.hnxiangtu.top

[R21] 字符串长度
来源：http://zrw.hysaishi.cn

echo "${#s}"
来源：http://foe.yj20258.top

[R22] 截取子串
来源：http://tfd.0kj1m.cn

echo "${s:0:5}"
来源：http://fjh.tarul.cn

[R23] 字符串替换
来源：http://fcy.yongpay.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dha.yueranfly.top

[R24] 大小写转换
来源：http://clj.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://xak.52xcode.cn

[R25] 去后缀 / 去前缀
来源：http://uch.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://key.ydjk.org.cn

[R26] 命令替换
来源：http://tnh.sweek.top

now=$(date +%F); echo "$now"
来源：http://bke.guannengcc.top

[R27] 算术展开
来源：http://lsp.shangyingyoupin.top

echo $((1 + 2 * 3))
来源：http://xpv.zhixingplan.top

[R28] 浮点运算
来源：http://fth.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://ast.gotoacloud.top

[R29] 定义函数
来源：http://udu.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ttx.shanyushiyangtech.top

[R30] 函数返回状态码
来源：http://uyu.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://bhi.yfazqb.com

[R31] 局部变量
来源：http://xkx.shangyingyoupin.top

f() { local x=1; echo "$x"; }
来源：http://bmz.shanyushiyangtech.top

[R32] 参数个数校验
来源：http://zka.hnqzz.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xix.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://ecp.sxryk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oru.mhx1999.top

[R34] 退出时清理
来源：http://puh.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rfy.jinqigfzy.top

[R35] 后台执行并等待
来源：http://udh.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://puz.ivvv.top

[R36] 并发执行多个任务
来源：http://hhl.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kyj.cdnleiting.top

[R37] 把输出赋给变量
来源：http://jbh.52xcode.cn

files=$(ls -1)
来源：http://uki.jianghu66.top

[R38] 管道串联
来源：http://tfw.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://jzn.pycfn.com

[R39] 重定向标准输出与错误
来源：http://jdy.zdbjq.cn

cmd > out.log 2>&1
来源：http://gur.meibo888.top

[R40] 追加写日志
来源：http://ppr.gaohongyu789.top

echo "log" >> out.log
来源：http://rpl.shanyushiyangkeji.top

[R41] 丢弃输出
来源：http://sbk.shuidangran.top

cmd >/dev/null 2>&1
来源：http://lgj.svipenyu.cn

[R42] 输入重定向
来源：http://sjj.yangfankeji.com

wc -l < a.txt
来源：http://cat.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://zbe.sysykeji.top

find . -name "*.log" -type f
来源：http://gtu.hammf.cn

[R44] 按修改时间查找
来源：http://qpw.ydzc1.top

find . -mtime -7 -type f
来源：http://cgm.aibaodan.cn

[R45] 批量删除
来源：http://fud.9152youxi.cn

find . -name "*.tmp" -delete
来源：http://uej.vehdjk.com

[R46] 递归替换文件内容
来源：http://mvm.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lzj.fzhhl.top

[R47] sed 单行替换
来源：http://qct.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://fyy.dianchejie.cn

[R48] awk 取指定列
来源：http://kqx.jianghu66.top

awk '{print $1, $3}' a.txt
来源：http://hpk.sxryk.cn

[R49] awk 带条件
来源：http://wms.dashuyun.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ups.hongshengwenyu.top

[R50] awk 求和
来源：http://hgv.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://ymd.snrcjt.cn

[R51] 排序去重取前几
来源：http://sma.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fan.hnqzz.top

[R52] 统计行数
来源：http://xzw.zdbjq.cn

wc -l a.txt
来源：http://msi.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://jxy.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://foc.daria6918.cn

[R54] 比较两个文件
来源：http://sxc.cdnleiting.top

diff a.txt b.txt
来源：http://pij.9152youxi.cn

[R55] 压缩与解压
来源：http://uvf.tarul.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jnn.gaohongyu789.top

[R56] 远程拷贝
来源：http://cbg.mhx1999.top

scp file user@host:/path/
来源：http://rai.andypj.xyz

[R57] 远程执行命令
来源：http://qth.yj202588.top

ssh user@host 'uptime'
来源：http://oth.yj202588.top

[R58] 下载文件
来源：http://czk.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ocm.guannengcc.top

[R59] 发 POST JSON
来源：http://rws.andypj.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ygt.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://dnh.nanxinkj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rht.gogol.net.cn

[R61] 磁盘占用
来源：http://eij.hesvh.cn

df -h;  du -sh *
来源：http://ycj.ybcxt.top

[R62] 找最占空间的文件
来源：http://crb.zdqjudy.top

du -ah . | sort -rh | head -10
来源：http://kpc.zhiwuduotai.top

[R63] 内存与进程
来源：http://kbf.meibo888.top

free -h;  ps aux | grep nginx
来源：http://aci.vqdsnc.cn

[R64] 结束进程
来源：http://wkd.pengpengdd.cyou

kill -9 $(pgrep -f app.py)
来源：http://awe.dashuyun.cn

[R65] 查看端口占用
来源：http://thd.kuanghao11.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://idi.yj20258888.top

[R66] 定时任务
来源：http://ydj.chenjidiqi.icu

crontab -e;  crontab -l
来源：http://tqy.tian-w.cn

[R67] 生成随机十六进制串
来源：http://def.feifeiyinyue.top

openssl rand -hex 16
来源：http://byv.cashguo.top

[R68] 计算文件校验值
来源：http://sqj.zhixingplan.top

sha256sum a.txt;  md5sum a.txt
来源：http://mht.yuanzhike.top

[R69] 生成随机密码
来源：http://kir.0kj1m.cn

head -c 16 /dev/urandom | base64
来源：http://svz.zycfv.cn

[R70] 时间戳与互转
来源：http://msy.yuxming.cn

date +%s;  date -d @1700000000
来源：http://vli.jqgfzy.top

[R71] 日期格式化
来源：http://wpp.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hjk.cucudq.cn

[R72] 等待端口就绪
来源：http://sue.52xcode.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cqx.snrcjt.cn

[R73] 分割大日志
来源：http://fhr.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://jjh.nanxinkj.top

[R74] 批量重命名
来源：http://kob.zhixingplan.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jhg.meibo888.top

[R75] 导出环境变量
来源：http://apx.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://kdh.pengpengdd.cyou

[R76] 使用临时文件
来源：http://aqo.haohaochexian.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ggv.sxryk.cn

[R77] 读取用户输入
来源：http://ndn.ppjwa.cn

read -rp "请输入: " ans
来源：http://wmx.nanxuanxn.top

[R78] 交互式菜单
来源：http://iod.ehwqpu.com

select opt in a b c; do echo "$opt"; break; done
来源：http://tns.iojbl.cn

[R79] 解析命令行选项
来源：http://faz.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ocy.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://wfv.feifeiyinyue.top

time ./run.sh
来源：http://fhl.tanke756.top

================================================================================
来源：http://oig.jinyuanbaomall.cn

S. C / C++ 专题
来源：http://bwh.epnwcf.com

================================================================================
来源：http://lta.hcnkem.com

[S01] C：Hello World
来源：http://lrh.bjfxy.top

#include <stdio.h>
来源：http://lin.havefunace.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ydd.jianghu66.top

[S02] C：变量与格式化输出
来源：http://hwt.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://lcu.gaohongyu789.top

[S03] C：读入整数
来源：http://nwr.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://vbd.yongpay.top

[S04] C：字符串复制
来源：http://lbp.cheryme.top

char dst[32]; strcpy(dst, "hi");
来源：http://aip.zhixingplan.top

[S05] C：字符串长度
来源：http://zgs.xuetiantiany.cn

strlen(s)
来源：http://eex.jqgfzy.top

[S06] C：字符串比较
来源：http://bhl.yonumen.top

strcmp(a, b) == 0
来源：http://mrr.mhx1999.top

[S07] C：数组遍历求和
来源：http://cuk.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ntv.0kj1m.cn

[S08] C：动态内存分配与释放
来源：http://cqz.yj20258.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lvn.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://ftb.dianchejie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qai.ivvv.top

[S10] C：指针与解引用
来源：http://xlj.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://cmc.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://rtq.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://qds.daria6918.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lnb.hongshengwenyu.top

fclose(f);
来源：http://uwc.yj20258888.top

[S12] C：写文件
来源：http://ulg.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jhc.meibo888.top

[S13] C：宏定义
来源：http://icp.andypj.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://drr.0kj1m.cn

[S14] C：枚举
来源：http://xej.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://jzd.gzhubu.top

[S15] C：类型转换
来源：http://pzj.jinqigfzy.top

(double) a / b
来源：http://fly.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://iql.vehdjk.com

x |= (1 << 3);
来源：http://riz.jianghu66.top

[S17] C：安全拼接字符串
来源：http://vav.sysykeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bth.ydjk.org.cn

[S18] C：命令行参数
来源：http://vcl.ydzc1.top

int main(int argc, char **argv)
来源：http://jen.sjlbkw.cn

[S19] C：快速排序
来源：http://bki.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nuf.hnqzz.top

[S20] C：二分查找
来源：http://dbw.kuanghao11.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qqs.tarul.cn

[S21] C：字符类别判断
来源：http://wbp.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xfb.hnxiangtu.top

[S22] C：字符串转数字
来源：http://pgf.uphjek.com

atoi("42");  strtod("3.14", NULL);
来源：http://jsj.52xcode.cn

[S23] C：随机数
来源：http://geq.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://aet.redwolf501.top

[S24] C：获取本地时间
来源：http://awd.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qqt.fktsv.cn

[S25] C：内存拷贝
来源：http://xte.gogol.net.cn

memcpy(dst, src, n);
来源：http://xyh.meibo888.top

[S26] C：内存清零
来源：http://jnz.hammf.cn

memset(a, 0, sizeof a);
来源：http://dea.yuanzhike.top

[S27] C：定义常量
来源：http://riw.havefunace.top

const double PI = 3.14159;
来源：http://zzk.xuetiantiany.cn

[S28] C：静态变量
来源：http://pqs.bbcook.cn

static int counter = 0;
来源：http://ccn.yangfankeji.com

[S29] C：变参函数
来源：http://xxa.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qps.zhongyouzk.top

[S30] C：头文件保护
来源：http://jzj.jqgfzy.top

#ifndef X_H
来源：http://umj.chenzaomai.com

#define X_H
来源：http://fsi.zdbjq.cn

#endif
来源：http://ozb.yangfankeji.com

[S31] C++：Hello World
来源：http://vlv.sufxvd.cn

#include <iostream>
来源：http://jkx.yj20258.top

int main() { std::cout << "Hello\n"; }
来源：http://mwh.hongshengwenyu.top

[S32] C++：字符串
来源：http://bpv.hammf.cn

std::string s = "hi";  s += "!";
来源：http://zrk.jiagoushi.top

[S33] C++：vector 增删
来源：http://obw.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zjm.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://pmo.aizwys.cn

for (auto &x : v) { std::cout << x; }
来源：http://lbj.yj202588.top

[S35] C++：map
来源：http://pkk.yvedp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bhs.shzxlz.cn

[S36] C++：unordered_map
来源：http://ksr.iojbl.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://roy.mhx1999.top

[S37] C++：set
来源：http://cwt.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rag.daxiang520.top

[S38] C++：排序
来源：http://avm.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://azn.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://cfe.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ysk.feifeiyinyue.top

[S40] C++：查找元素
来源：http://yjk.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://enn.gotoacloud.top

[S41] C++：类与构造函数
来源：http://kgs.epnwcf.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jdd.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://xfr.andypj.xyz

class B : public Base { public: void f() override {} };
来源：http://tdh.hfpthk.cn

[S43] C++：智能指针
来源：http://tfg.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://bds.redwolf501.top

[S44] C++：引用传参
来源：http://nfg.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://ceq.zdqjudy.top

[S45] C++：lambda
来源：http://scu.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tfl.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://cwr.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dwg.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://tri.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ebi.shanyushiyangtech.top

[S48] C++：逐行读文件
来源：http://cxd.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://roj.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://srk.xylfe.cn

[S49] C++：写文件
来源：http://vsc.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nlr.fanxiaobao.xyz

[S50] C++：格式化数字
来源：http://idm.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pcm.yuanzhike.top

[S51] C++：显式类型转换
来源：http://ops.pycfn.com

static_cast<double>(a) / b
来源：http://cuz.sweek.top

[S52] C++：const 与 noexcept
来源：http://lju.tarul.cn

int size() const noexcept { return n_; }
来源：http://spg.bbcook.cn

[S53] C++：移动语义
来源：http://kyd.yongpay.top

std::vector<int> w = std::move(v);
来源：http://tuu.cheryme.top

[S54] C++：异常处理
来源：http://cpn.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zvx.sysykeji.top

[S55] C++：结构化绑定
来源：http://xeg.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oid.sweek.top

[S56] C++：optional
来源：http://apd.hywenlv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bak.dianchejie.cn

[S57] C++：编译期常量
来源：http://typ.shzxlz.cn

constexpr int N = 10;
来源：http://xtt.andypj.xyz

[S58] C++：命名空间
来源：http://qyv.shuidangran.top

namespace ns { int f() { return 1; } }
来源：http://lxz.zhijiandao.cn

[S59] C++：静态断言
来源：http://cks.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kqc.meibo888.top

[S60] C++：遍历并删除元素
来源：http://rnr.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vtw.chenjidiqi.icu

================================================================================
来源：http://lbk.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wje.c1oappe.top

================================================================================
来源：http://hpk.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://cpz.hcnkem.com

println("Hello")
来源：http://cfr.jinqigufen.top

[T02] Kotlin：变量
来源：http://vhv.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zbt.yueranfly.top

[T03] Kotlin：字符串模板
来源：http://ytb.nanxuanxn.top

"值: $b"
来源：http://gom.haohaochexian.top

[T04] Kotlin：空安全
来源：http://gqb.daxiang520.top

val n: String? = null;  n?.length
来源：http://dmr.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://cbs.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cxy.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://xws.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://woy.yueranfly.top

[T07] Kotlin：集合过滤
来源：http://gvo.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vej.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://sen.vehdjk.com

data class User(val name: String, val age: Int)
来源：http://plw.bbcook.cn

[T09] Kotlin：扩展函数
来源：http://yls.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://fmw.nanxinkj.top

[T10] Kotlin：默认参数
来源：http://win.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://znt.aibaodan.cn

[T11] Kotlin：协程
来源：http://xag.hnqzz.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jdp.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://yav.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://ruv.yj202588.top

[T13] Kotlin：只读 Map
来源：http://upa.yanxiufei.cn

val m = mapOf("a" to 1)
来源：http://bia.yueranfly.top

[T14] Kotlin：循环
来源：http://fmu.jinqigfzy.top

for (i in 1..10) println(i)
来源：http://shq.svipenyu.cn


<!-- 参考信息 -->