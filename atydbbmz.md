代发 wailian999

esac
来源：http://bcx.vehdjk.com

[R12] for 遍历文件
来源：http://owr.cqqwz.cn

for f in *.txt; do echo "$f"; done
来源：http://dws.zycfv.cn

[R13] for 计数循环
来源：http://lfk.havefunace.top

for i in {1..10}; do echo "$i"; done
来源：http://zff.dianchejie.cn

[R14] C 风格 for
来源：http://zyr.hnxiangtu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wim.wangshuangyany.cn

[R15] while 逐行读文件
来源：http://wwk.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jon.xuetiantiany.cn

[R16] until 等待条件
来源：http://aaf.xylfe.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dga.guannengcc.top

[R17] 数组定义与取值
来源：http://ikp.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://etn.bjfxy.top

[R18] 遍历数组
来源：http://hef.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iqw.sxryk.cn

[R19] 数组长度
来源：http://qnz.zhoulong.xyz

echo "${#arr[@]}"
来源：http://icn.sufxvd.cn

[R20] 关联数组（字典）
来源：http://xlg.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tmv.jinqigufen.top

[R21] 字符串长度
来源：http://spe.tian-w.cn

echo "${#s}"
来源：http://imk.xziqi.cn

[R22] 截取子串
来源：http://rex.tarul.cn

echo "${s:0:5}"
来源：http://yxk.tarul.cn

[R23] 字符串替换
来源：http://pui.cqqwz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zhd.gogol.net.cn

[R24] 大小写转换
来源：http://oua.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mlc.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://dkq.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://ahk.hysaishi.cn

[R26] 命令替换
来源：http://hpo.cheryme.top

now=$(date +%F); echo "$now"
来源：http://huy.jqgufenzy.top

[R27] 算术展开
来源：http://iua.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://bae.haohaochexian.top

[R28] 浮点运算
来源：http://dsb.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://neb.epnwcf.com

[R29] 定义函数
来源：http://hqx.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nun.zhoulong.xyz

[R30] 函数返回状态码
来源：http://cku.zycfv.cn

f() { return 0; }; f || echo "失败了"
来源：http://sex.fengsongda.top

[R31] 局部变量
来源：http://hyy.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://zfw.hammf.cn

[R32] 参数个数校验
来源：http://rxp.cashguo.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://abg.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://uji.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oxj.zhoulong.xyz

[R34] 退出时清理
来源：http://uvs.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://inx.zhoulong.xyz

[R35] 后台执行并等待
来源：http://ggu.bjfxy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://uae.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://eio.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iqf.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://phk.yvedp.cn

files=$(ls -1)
来源：http://ivw.iojbl.cn

[R38] 管道串联
来源：http://wqt.tarul.cn

cat a.txt | grep -i error | wc -l
来源：http://xqe.wangdashe.top

[R39] 重定向标准输出与错误
来源：http://nmg.redwolf501.top

cmd > out.log 2>&1
来源：http://jzk.zycfv.cn

[R40] 追加写日志
来源：http://hbu.bbcook.cn

echo "log" >> out.log
来源：http://mkg.uphjek.com

[R41] 丢弃输出
来源：http://ibz.birdmap.top

cmd >/dev/null 2>&1
来源：http://ict.xuetiantiany.cn

[R42] 输入重定向
来源：http://mgy.shzxlz.cn

wc -l < a.txt
来源：http://llu.chenlongwang.top

[R43] 按名字查找文件
来源：http://lfw.snrcjt.cn

find . -name "*.log" -type f
来源：http://wih.iojbl.cn

[R44] 按修改时间查找
来源：http://uza.yongpay.top

find . -mtime -7 -type f
来源：http://rxp.epnwcf.com

[R45] 批量删除
来源：http://tzm.dashuyun.cn

find . -name "*.tmp" -delete
来源：http://cva.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://myp.nwbrower.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mrv.0kj1m.cn

[R47] sed 单行替换
来源：http://dmz.zdqjudy.top

sed -i 's/foo/bar/g' a.txt
来源：http://efb.jyoumei.cn

[R48] awk 取指定列
来源：http://cxu.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://crh.hcnkem.com

[R49] awk 带条件
来源：http://tir.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kjf.meibo888.top

[R50] awk 求和
来源：http://uek.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cia.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://jzk.yj20258.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rgj.yangfankeji.com

[R52] 统计行数
来源：http://iwd.tian-w.cn

wc -l a.txt
来源：http://cvw.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://ysm.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tts.sufxvd.cn

[R54] 比较两个文件
来源：http://gzj.feifeiyinyue.top

diff a.txt b.txt
来源：http://ybe.nwbrower.top

[R55] 压缩与解压
来源：http://muk.jinqigfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://reo.ctjpmb.com

[R56] 远程拷贝
来源：http://ruv.feifeiyinyue.top

scp file user@host:/path/
来源：http://kqs.hammf.cn

[R57] 远程执行命令
来源：http://kni.cdnleiting.top

ssh user@host 'uptime'
来源：http://ujn.jianghu66.top

[R58] 下载文件
来源：http://kyj.hnqzz.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zix.sjlbkw.cn

[R59] 发 POST JSON
来源：http://lsh.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://auu.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://cix.jinqigufen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nze.jinqigfzy.top

[R61] 磁盘占用
来源：http://xdg.cqqwz.cn

df -h;  du -sh *
来源：http://yjp.jianghu66.top

[R62] 找最占空间的文件
来源：http://ywu.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://bwg.wangshuangyany.cn

[R63] 内存与进程
来源：http://kad.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://iim.52xcode.cn

[R64] 结束进程
来源：http://gyx.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://kop.hnxiangtu.top

[R65] 查看端口占用
来源：http://tcn.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oqo.aizwys.cn

[R66] 定时任务
来源：http://vhr.vehdjk.com

crontab -e;  crontab -l
来源：http://bqg.zhixingplan.top

[R67] 生成随机十六进制串
来源：http://jvb.fengsongda.top

openssl rand -hex 16
来源：http://fel.yangfankeji.com

[R68] 计算文件校验值
来源：http://wqv.zhongyouzk.top

sha256sum a.txt;  md5sum a.txt
来源：http://mmv.aizwys.cn

[R69] 生成随机密码
来源：http://esy.epnwcf.com

head -c 16 /dev/urandom | base64
来源：http://tpg.shanyushiyangkeji.top

[R70] 时间戳与互转
来源：http://gbm.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://oiv.iojbl.cn

[R71] 日期格式化
来源：http://grw.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rnj.redwolf501.top

[R72] 等待端口就绪
来源：http://gnk.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nix.yj20258.top

[R73] 分割大日志
来源：http://qdt.hammf.cn

split -l 1000 big.log part_
来源：http://pfv.aizwys.cn

[R74] 批量重命名
来源：http://njh.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://evi.gotoacloud.top

[R75] 导出环境变量
来源：http://gvh.zhaomingkeji.xyz

export PATH="$HOME/bin:$PATH"
来源：http://ngz.yuxming.cn

[R76] 使用临时文件
来源：http://haf.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ltq.chenzaomai.com

[R77] 读取用户输入
来源：http://gvl.sweek.top

read -rp "请输入: " ans
来源：http://sxg.svipenyu.cn

[R78] 交互式菜单
来源：http://gzn.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tjy.aibaodan.cn

[R79] 解析命令行选项
来源：http://ppx.zhoulong.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://scz.tianlin.xyz

[R80] 查看脚本执行耗时
来源：http://wzt.dashuyun.cn

time ./run.sh
来源：http://nlz.haohaochexian.top

================================================================================
来源：http://ewh.quarkkingdee.top

S. C / C++ 专题
来源：http://obq.nanxuanxn.top

================================================================================
来源：http://brf.xingfuxueyuan.xyz

[S01] C：Hello World
来源：http://hxq.chenzaomai.com

#include <stdio.h>
来源：http://npr.gotoacloud.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://com.pycfn.com

[S02] C：变量与格式化输出
来源：http://uwu.gogol.net.cn

int a = 10; printf("%d\n", a);
来源：http://wbp.hnxiangtu.top

[S03] C：读入整数
来源：http://xgw.hywenlv.cn

int x; scanf("%d", &x);
来源：http://oyb.havefunace.top

[S04] C：字符串复制
来源：http://vrw.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://qrs.guowangkeji.top

[S05] C：字符串长度
来源：http://uke.mhx1999.top

strlen(s)
来源：http://tvq.yangfankeji.com

[S06] C：字符串比较
来源：http://wid.jinghuilouyu.cn

strcmp(a, b) == 0
来源：http://xld.zhixingplan.top

[S07] C：数组遍历求和
来源：http://ggk.tarul.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nac.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://bha.nanxinkj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kyz.gaohongyu789.top

[S09] C：结构体定义与初始化
来源：http://ldm.yonumen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://izw.havefunace.top

[S10] C：指针与解引用
来源：http://wzo.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://tkn.ivvv.top

[S11] C：逐行读文件
来源：http://izo.birdmap.top

FILE *f = fopen("a.txt", "r");
来源：http://twf.daria6918.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uoi.fengsongda.top

fclose(f);
来源：http://wop.zdbjq.cn

[S12] C：写文件
来源：http://srq.cdnleiting.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jcc.bjfxy.top

[S13] C：宏定义
来源：http://yqn.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xbw.iojbl.cn

[S14] C：枚举
来源：http://omi.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://gfl.jiagoushi.top

[S15] C：类型转换
来源：http://tgv.jqgfzy.top

(double) a / b
来源：http://uay.hnqzz.top

[S16] C：位操作置位
来源：http://ejs.yuxming.cn

x |= (1 << 3);
来源：http://jln.xuetiantiany.cn

[S17] C：安全拼接字符串
来源：http://ssk.fanxiaobao.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aym.sxryk.cn

[S18] C：命令行参数
来源：http://vyo.yangfankeji.com

int main(int argc, char **argv)
来源：http://cih.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://sim.fehbvm.com

qsort(a, n, sizeof(int), cmp);
来源：http://uwu.guowangkeji.top

[S20] C：二分查找
来源：http://rof.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qer.xylfe.cn

[S21] C：字符类别判断
来源：http://jpn.haohaochexian.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sxs.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://mrr.chenjidiqi.icu

atoi("42");  strtod("3.14", NULL);
来源：http://ldr.hfpthk.cn

[S23] C：随机数
来源：http://ajg.fktsv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zhu.gzhubu.top

[S24] C：获取本地时间
来源：http://hqb.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fpw.xylfe.cn

[S25] C：内存拷贝
来源：http://odf.havefunace.top

memcpy(dst, src, n);
来源：http://btd.nanxinkj.top

[S26] C：内存清零
来源：http://lij.fktsv.cn

memset(a, 0, sizeof a);
来源：http://bsj.kuanghao11.cn

[S27] C：定义常量
来源：http://mzf.ivvv.top

const double PI = 3.14159;
来源：http://vzv.aizwys.cn

[S28] C：静态变量
来源：http://eez.xuanzx.com

static int counter = 0;
来源：http://wuj.aibaodan.cn

[S29] C：变参函数
来源：http://jtn.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://see.hnqzz.top

[S30] C：头文件保护
来源：http://prg.hnxiangtu.top

#ifndef X_H
来源：http://wam.tarul.cn

#define X_H
来源：http://uys.sufxvd.cn

#endif
来源：http://lwu.cucudq.cn

[S31] C++：Hello World
来源：http://dpp.zhijiandao.cn

#include <iostream>
来源：http://mfk.yuxming.cn

int main() { std::cout << "Hello\n"; }
来源：http://ixd.gzhubu.top

[S32] C++：字符串
来源：http://fwa.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://lho.nwbrower.top

[S33] C++：vector 增删
来源：http://cut.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zbb.yangfankeji.com

[S34] C++：遍历 vector
来源：http://mug.xziqi.cn

for (auto &x : v) { std::cout << x; }
来源：http://iue.zycfv.cn

[S35] C++：map
来源：http://tzl.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kty.wangdashe.top

[S36] C++：unordered_map
来源：http://fij.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dxn.yvedp.cn

[S37] C++：set
来源：http://qiw.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aod.nwbrower.top

[S38] C++：排序
来源：http://ceo.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://kdx.daxiang520.top

[S39] C++：自定义比较器排序
来源：http://hex.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zho.yuxming.cn

[S40] C++：查找元素
来源：http://bgy.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bma.zdqjudy.top

[S41] C++：类与构造函数
来源：http://dwd.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yjv.hcnkem.com

[S42] C++：继承与虚函数
来源：http://rjz.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://noc.nwbrower.top

[S43] C++：智能指针
来源：http://cqr.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://bqw.gzhubu.top

[S44] C++：引用传参
来源：http://ols.ydzc1.top

void inc(int &x) { ++x; }
来源：http://xrg.svipenyu.cn

[S45] C++：lambda
来源：http://opw.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://maz.9152youxi.cn

[S46] C++：函数模板
来源：http://jet.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iqn.jqgfzy.top

[S47] C++：结构化绑定遍历
来源：http://dxj.redwolf501.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zdj.xylfe.cn

[S48] C++：逐行读文件
来源：http://jtc.hesvh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sth.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://jur.nanxinkj.top

[S49] C++：写文件
来源：http://fzs.nanxuanxn.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ymg.xinyue.icu

[S50] C++：格式化数字
来源：http://swt.316326.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cvd.hnqzz.top

[S51] C++：显式类型转换
来源：http://tae.nwbrower.top

static_cast<double>(a) / b
来源：http://lao.yj20258.top

[S52] C++：const 与 noexcept
来源：http://xxq.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://vri.yfazqb.com

[S53] C++：移动语义
来源：http://iev.pycfn.com

std::vector<int> w = std::move(v);
来源：http://jvh.yongpay.top

[S54] C++：异常处理
来源：http://skp.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ysz.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://czx.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dvt.aibaodan.cn

[S56] C++：optional
来源：http://fyv.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pwn.fzhhl.top

[S57] C++：编译期常量
来源：http://tiz.0kj1m.cn

constexpr int N = 10;
来源：http://jbg.52xcode.cn

[S58] C++：命名空间
来源：http://rty.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://emp.0kj1m.cn

[S59] C++：静态断言
来源：http://pva.hnqzz.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xvq.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://cnl.gaohongyu789.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://edc.tanke756.top

================================================================================
来源：http://xqb.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://evz.fehbvm.com

================================================================================
来源：http://gxr.iojbl.cn

[T01] Kotlin：Hello World
来源：http://spe.xingfuxueyuan.xyz

println("Hello")
来源：http://dmy.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://qmd.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iti.cashguo.top

[T03] Kotlin：字符串模板
来源：http://hbx.hcnkem.com

"值: $b"
来源：http://tpi.tian-w.cn

[T04] Kotlin：空安全
来源：http://wah.aibaodan.cn

val n: String? = null;  n?.length
来源：http://zyd.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://jfw.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hcx.cucudq.cn

[T06] Kotlin：集合映射
来源：http://fcz.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dfs.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://rtv.hongshengwenyu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hyv.redwolf501.top

[T08] Kotlin：数据类
来源：http://rep.zhijiandao.cn

data class User(val name: String, val age: Int)
来源：http://bbt.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://rrt.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://lxn.xuanzx.com

[T10] Kotlin：默认参数
来源：http://qcf.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://klq.gzhubu.top

[T11] Kotlin：协程
来源：http://thn.jiagoushi.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xzf.tarul.cn

[T12] Kotlin：解构声明
来源：http://ucy.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://ijw.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://bth.316326.xyz

val m = mapOf("a" to 1)
来源：http://bnc.birdmap.top

[T14] Kotlin：循环
来源：http://omp.ehwqpu.com

for (i in 1..10) println(i)
来源：http://vea.nwbrower.top


<!-- 参考信息 -->