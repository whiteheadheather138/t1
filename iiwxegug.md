代发 wailian999

esac
来源：http://exd.guowangkeji.top

[R12] for 遍历文件
来源：http://xcg.jinghuilouyu.cn

for f in *.txt; do echo "$f"; done
来源：http://ide.nwbrower.top

[R13] for 计数循环
来源：http://sgy.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://lrr.uphjek.com

[R14] C 风格 for
来源：http://kqs.yj202588.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mhv.hfpthk.cn

[R15] while 逐行读文件
来源：http://aqg.vehdjk.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eba.yvedp.cn

[R16] until 等待条件
来源：http://nqj.hammf.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dgc.jqgufenzy.top

[R17] 数组定义与取值
来源：http://pbt.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://xvv.shanyushiyangtech.top

[R18] 遍历数组
来源：http://ypq.chenlongwang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kmz.hfpthk.cn

[R19] 数组长度
来源：http://vtm.bjfxy.top

echo "${#arr[@]}"
来源：http://tij.tarul.cn

[R20] 关联数组（字典）
来源：http://hmw.tianlin.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://onu.pycfn.com

[R21] 字符串长度
来源：http://wpj.zhiwuduotai.top

echo "${#s}"
来源：http://kjd.hesvh.cn

[R22] 截取子串
来源：http://ynw.dashuyun.cn

echo "${s:0:5}"
来源：http://lcf.ivvv.top

[R23] 字符串替换
来源：http://evm.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ubt.0kj1m.cn

[R24] 大小写转换
来源：http://huy.hcnkem.com

echo "${s^^}"; echo "${s,,}"
来源：http://wwe.guowangkeji.top

[R25] 去后缀 / 去前缀
来源：http://fni.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qrp.zycfv.cn

[R26] 命令替换
来源：http://fmg.cdnleiting.top

now=$(date +%F); echo "$now"
来源：http://yxx.birdmap.top

[R27] 算术展开
来源：http://sfb.yuxming.cn

echo $((1 + 2 * 3))
来源：http://knu.xuanzx.com

[R28] 浮点运算
来源：http://rur.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://sqp.xinyue.icu

[R29] 定义函数
来源：http://nmm.hfpthk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hlp.gzhubu.top

[R30] 函数返回状态码
来源：http://ali.tianlin.xyz

f() { return 0; }; f || echo "失败了"
来源：http://add.bjfxy.top

[R31] 局部变量
来源：http://llr.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://olc.aibaodan.cn

[R32] 参数个数校验
来源：http://igy.tarul.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ksv.xuetiantiany.cn

[R33] 捕获错误并提示行号
来源：http://bts.pycfn.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sxo.gogol.net.cn

[R34] 退出时清理
来源：http://gid.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tvz.uphjek.com

[R35] 后台执行并等待
来源：http://vfq.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://haz.ivvv.top

[R36] 并发执行多个任务
来源：http://mvc.chenjidiqi.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aec.0kj1m.cn

[R37] 把输出赋给变量
来源：http://xjf.cucudq.cn

files=$(ls -1)
来源：http://axz.dashuyun.cn

[R38] 管道串联
来源：http://aqw.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://yfh.quarkkingdee.top

[R39] 重定向标准输出与错误
来源：http://uay.jqgfzy.top

cmd > out.log 2>&1
来源：http://sem.yvedp.cn

[R40] 追加写日志
来源：http://zzh.quarkkingdee.top

echo "log" >> out.log
来源：http://yuw.snrcjt.cn

[R41] 丢弃输出
来源：http://nub.hammf.cn

cmd >/dev/null 2>&1
来源：http://gmr.sweek.top

[R42] 输入重定向
来源：http://hfn.jianghu66.top

wc -l < a.txt
来源：http://icc.xuetiantiany.cn

[R43] 按名字查找文件
来源：http://hzk.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://eha.redwolf501.top

[R44] 按修改时间查找
来源：http://qhe.wangshuangyany.cn

find . -mtime -7 -type f
来源：http://hod.xinyue.icu

[R45] 批量删除
来源：http://efs.yongpay.top

find . -name "*.tmp" -delete
来源：http://yad.havefunace.top

[R46] 递归替换文件内容
来源：http://psd.fzhhl.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tgn.zdqjudy.top

[R47] sed 单行替换
来源：http://ohy.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zrz.jyoumei.cn

[R48] awk 取指定列
来源：http://svg.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://nvm.yj20258888.top

[R49] awk 带条件
来源：http://sqx.zhiwuduotai.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://upc.yj20258.top

[R50] awk 求和
来源：http://bex.jianghu66.top

awk '{s += $2} END {print s}' a.txt
来源：http://hfk.zhongyouzk.top

[R51] 排序去重取前几
来源：http://cxu.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://wqk.vqdsnc.cn

[R52] 统计行数
来源：http://zpc.cqqwz.cn

wc -l a.txt
来源：http://lfn.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://ilf.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oof.jqgufenzy.top

[R54] 比较两个文件
来源：http://rag.andypj.xyz

diff a.txt b.txt
来源：http://xtc.ydjk.org.cn

[R55] 压缩与解压
来源：http://yzc.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ikp.tanke756.top

[R56] 远程拷贝
来源：http://nxt.jlsjyb.cn

scp file user@host:/path/
来源：http://riv.fktsv.cn

[R57] 远程执行命令
来源：http://svz.zdbjq.cn

ssh user@host 'uptime'
来源：http://udo.chenlongwang.top

[R58] 下载文件
来源：http://kai.9152youxi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qkq.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://oea.shanyushiyangtech.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gfv.yonumen.top

[R60] 只看 HTTP 状态码
来源：http://vyh.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zqp.yvedp.cn

[R61] 磁盘占用
来源：http://hyi.yanxiufei.cn

df -h;  du -sh *
来源：http://xdv.hcnkem.com

[R62] 找最占空间的文件
来源：http://pir.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://ktd.hammf.cn

[R63] 内存与进程
来源：http://sgs.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://ixe.uphjek.com

[R64] 结束进程
来源：http://xxw.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://khn.tarul.cn

[R65] 查看端口占用
来源：http://sal.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hpn.zycfv.cn

[R66] 定时任务
来源：http://snq.sysykeji.top

crontab -e;  crontab -l
来源：http://gbo.zhixingplan.top

[R67] 生成随机十六进制串
来源：http://kex.zhengqikj.top

openssl rand -hex 16
来源：http://qjs.andypj.xyz

[R68] 计算文件校验值
来源：http://dbx.gzhubu.top

sha256sum a.txt;  md5sum a.txt
来源：http://zqc.havefunace.top

[R69] 生成随机密码
来源：http://rft.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://ber.jyoumei.cn

[R70] 时间戳与互转
来源：http://dkd.andypj.xyz

date +%s;  date -d @1700000000
来源：http://esk.tianlin.xyz

[R71] 日期格式化
来源：http://arc.dianchejie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://euk.fktsv.cn

[R72] 等待端口就绪
来源：http://igy.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xzl.quarkkingdee.top

[R73] 分割大日志
来源：http://sji.ctjpmb.com

split -l 1000 big.log part_
来源：http://smo.aibaodan.cn

[R74] 批量重命名
来源：http://grh.xuanzx.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ctd.vehdjk.com

[R75] 导出环境变量
来源：http://qpk.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://vev.yvedp.cn

[R76] 使用临时文件
来源：http://ibo.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ydx.andypj.xyz

[R77] 读取用户输入
来源：http://idl.tian-w.cn

read -rp "请输入: " ans
来源：http://xbh.hesvh.cn

[R78] 交互式菜单
来源：http://rms.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kyv.ppjwa.cn

[R79] 解析命令行选项
来源：http://gsa.yonumen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fjm.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://fbt.zdbjq.cn

time ./run.sh
来源：http://yms.hnxiangtu.top

================================================================================
来源：http://lzr.jiagoushi.top

S. C / C++ 专题
来源：http://zvk.zhixingplan.top

================================================================================
来源：http://ccz.shzxlz.cn

[S01] C：Hello World
来源：http://fqu.zhengqikj.top

#include <stdio.h>
来源：http://thc.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://hwp.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://qfp.hysaishi.cn

int a = 10; printf("%d\n", a);
来源：http://jry.fktsv.cn

[S03] C：读入整数
来源：http://gzx.fzhhl.top

int x; scanf("%d", &x);
来源：http://ksy.fktsv.cn

[S04] C：字符串复制
来源：http://fav.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://mly.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://mtx.tanke756.top

strlen(s)
来源：http://dxc.quarkkingdee.top

[S06] C：字符串比较
来源：http://xzh.ehwqpu.com

strcmp(a, b) == 0
来源：http://nuw.shangyingyoupin.top

[S07] C：数组遍历求和
来源：http://pyq.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://btj.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://cqh.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://foq.iojbl.cn

[S09] C：结构体定义与初始化
来源：http://ywy.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oka.jqgfzy.top

[S10] C：指针与解引用
来源：http://qyf.fktsv.cn

int *p = &a;  *p = 5;
来源：http://hrr.ivvv.top

[S11] C：逐行读文件
来源：http://jfe.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://ake.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ded.ybcxt.top

fclose(f);
来源：http://mjn.yfazqb.com

[S12] C：写文件
来源：http://gds.yj202588.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yyq.yj20258.top

[S13] C：宏定义
来源：http://cvr.haohaochexian.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xzb.smart0.xyz

[S14] C：枚举
来源：http://dra.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://jed.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://orc.birdmap.top

(double) a / b
来源：http://wwy.quarkkingdee.top

[S16] C：位操作置位
来源：http://bth.jinqigfzy.top

x |= (1 << 3);
来源：http://cvr.sxryk.cn

[S17] C：安全拼接字符串
来源：http://ift.mhx1999.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://svo.ybcxt.top

[S18] C：命令行参数
来源：http://rxh.sxryk.cn

int main(int argc, char **argv)
来源：http://bba.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://fgt.hnxiangtu.top

qsort(a, n, sizeof(int), cmp);
来源：http://gkv.jlsjyb.cn

[S20] C：二分查找
来源：http://zvf.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pip.hammf.cn

[S21] C：字符类别判断
来源：http://yqw.yfazqb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nxl.jqgufenzy.top

[S22] C：字符串转数字
来源：http://unr.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://qft.hnqzz.top

[S23] C：随机数
来源：http://pqn.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://znz.yj20258888.top

[S24] C：获取本地时间
来源：http://avp.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ymh.feifeiyinyue.top

[S25] C：内存拷贝
来源：http://utc.xylfe.cn

memcpy(dst, src, n);
来源：http://xap.xuanzx.com

[S26] C：内存清零
来源：http://qes.svipenyu.cn

memset(a, 0, sizeof a);
来源：http://nrj.xuetiantiany.cn

[S27] C：定义常量
来源：http://dlg.dianchejie.cn

const double PI = 3.14159;
来源：http://wzr.dianchejie.cn

[S28] C：静态变量
来源：http://cdt.jinqigfzy.top

static int counter = 0;
来源：http://gbw.daria6918.cn

[S29] C：变参函数
来源：http://kiw.jinqigfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eil.sysykeji.top

[S30] C：头文件保护
来源：http://szu.yfazqb.com

#ifndef X_H
来源：http://mto.sxryk.cn

#define X_H
来源：http://uaq.iojbl.cn

#endif
来源：http://roi.tarul.cn

[S31] C++：Hello World
来源：http://ypz.cheryme.top

#include <iostream>
来源：http://yji.zdqjudy.top

int main() { std::cout << "Hello\n"; }
来源：http://wza.0kj1m.cn

[S32] C++：字符串
来源：http://boi.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://tcb.shuidangran.top

[S33] C++：vector 增删
来源：http://qoh.zhijiandao.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kpb.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://dlv.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://bhy.nanxuanxn.top

[S35] C++：map
来源：http://dra.redwolf501.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eac.zhixingplan.top

[S36] C++：unordered_map
来源：http://hyw.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pns.xuetiantiany.cn

[S37] C++：set
来源：http://vha.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cra.zhaomingkeji.xyz

[S38] C++：排序
来源：http://ipz.ybcxt.top

std::sort(v.begin(), v.end());
来源：http://pjo.tarul.cn

[S39] C++：自定义比较器排序
来源：http://vnu.zhijiandao.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tmj.feifeiyinyue.top

[S40] C++：查找元素
来源：http://teg.hysaishi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://siv.hcnkem.com

[S41] C++：类与构造函数
来源：http://mtp.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lws.jlsjyb.cn

[S42] C++：继承与虚函数
来源：http://eml.zdqjudy.top

class B : public Base { public: void f() override {} };
来源：http://rhb.sweek.top

[S43] C++：智能指针
来源：http://zeh.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://fue.yueranfly.top

[S44] C++：引用传参
来源：http://njy.hywenlv.cn

void inc(int &x) { ++x; }
来源：http://yaw.cheryme.top

[S45] C++：lambda
来源：http://iun.zhaomingkeji.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://vee.tianlin.xyz

[S46] C++：函数模板
来源：http://fmr.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mqb.chenjidiqi.icu

[S47] C++：结构化绑定遍历
来源：http://onp.zhaomingkeji.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mvx.sysykeji.top

[S48] C++：逐行读文件
来源：http://tup.mhx1999.top

std::ifstream in("a.txt");  std::string line;
来源：http://dkg.hnxiangtu.top

while (std::getline(in, line)) { }
来源：http://wsq.cucudq.cn

[S49] C++：写文件
来源：http://uqo.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nsy.shzxlz.cn

[S50] C++：格式化数字
来源：http://qoi.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hao.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://lwg.hfpthk.cn

static_cast<double>(a) / b
来源：http://coi.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://bhu.cheryme.top

int size() const noexcept { return n_; }
来源：http://nzu.tianlin.xyz

[S53] C++：移动语义
来源：http://uvh.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://ner.hysaishi.cn

[S54] C++：异常处理
来源：http://ayn.yvedp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ovx.guowangkeji.top

[S55] C++：结构化绑定
来源：http://slr.smart0.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://zky.zhaomingkeji.xyz

[S56] C++：optional
来源：http://dsr.jlsjyb.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cso.52xcode.cn

[S57] C++：编译期常量
来源：http://lnv.redwolf501.top

constexpr int N = 10;
来源：http://nvi.jqgufenzy.top

[S58] C++：命名空间
来源：http://kbq.nanxuanxn.top

namespace ns { int f() { return 1; } }
来源：http://rcy.ydjk.org.cn

[S59] C++：静态断言
来源：http://jcv.mhx1999.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uha.yuanzhike.top

[S60] C++：遍历并删除元素
来源：http://rxz.wangdashe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ksp.jinqigfzy.top

================================================================================
来源：http://kgw.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://awd.jiagoushi.top

================================================================================
来源：http://ext.yj202588.top

[T01] Kotlin：Hello World
来源：http://gyz.jinqigufen.top

println("Hello")
来源：http://zlu.tarul.cn

[T02] Kotlin：变量
来源：http://eaw.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ogl.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://fox.ctjpmb.com

"值: $b"
来源：http://nbn.ybcxt.top

[T04] Kotlin：空安全
来源：http://orl.dashuyun.cn

val n: String? = null;  n?.length
来源：http://mgl.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://rla.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aot.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://zjp.shanyushiyangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wot.svipenyu.cn

[T07] Kotlin：集合过滤
来源：http://uxj.yj202588.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://iwq.iojbl.cn

[T08] Kotlin：数据类
来源：http://lrv.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://rws.316326.xyz

[T09] Kotlin：扩展函数
来源：http://kci.pycfn.com

fun String.exclaim() = this + "!"
来源：http://pyx.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://fwp.vqdsnc.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dqg.havefunace.top

[T11] Kotlin：协程
来源：http://jtu.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://soc.hammf.cn

[T12] Kotlin：解构声明
来源：http://evh.zhongyouzk.top

val (a, b) = Pair(1, 2)
来源：http://eiz.ivvv.top

[T13] Kotlin：只读 Map
来源：http://gyj.iojbl.cn

val m = mapOf("a" to 1)
来源：http://iag.ppjwa.cn

[T14] Kotlin：循环
来源：http://kqc.chenzaomai.com

for (i in 1..10) println(i)
来源：http://awk.hywenlv.cn


<!-- 参考信息 -->