代发 wailian999

esac
来源：http://rtf.9152youxi.cn

[R12] for 遍历文件
来源：http://vch.hnxiangtu.top

for f in *.txt; do echo "$f"; done
来源：http://irj.52xcode.cn

[R13] for 计数循环
来源：http://vmj.yj20258888.top

for i in {1..10}; do echo "$i"; done
来源：http://kpz.ydzc1.top

[R14] C 风格 for
来源：http://ump.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jjz.sufxvd.cn

[R15] while 逐行读文件
来源：http://tyx.hesvh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ndn.yonumen.top

[R16] until 等待条件
来源：http://vml.yuanzhike.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lyq.chenlongwang.top

[R17] 数组定义与取值
来源：http://dpm.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://hax.cashguo.top

[R18] 遍历数组
来源：http://axx.bjfxy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://npq.meibo888.top

[R19] 数组长度
来源：http://slf.svipenyu.cn

echo "${#arr[@]}"
来源：http://dgg.cashguo.top

[R20] 关联数组（字典）
来源：http://yha.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ujh.hywenlv.cn

[R21] 字符串长度
来源：http://jbp.shzxlz.cn

echo "${#s}"
来源：http://tyn.yanxiufei.cn

[R22] 截取子串
来源：http://bnw.yuxming.cn

echo "${s:0:5}"
来源：http://tll.hnqzz.top

[R23] 字符串替换
来源：http://ptx.hcnkem.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qxb.quarkkingdee.top

[R24] 大小写转换
来源：http://fpn.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qka.zhijiandao.cn

[R25] 去后缀 / 去前缀
来源：http://ymd.quarkkingdee.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fpo.yj202588.top

[R26] 命令替换
来源：http://vlc.hnxiangtu.top

now=$(date +%F); echo "$now"
来源：http://ksx.yuxming.cn

[R27] 算术展开
来源：http://nav.sxryk.cn

echo $((1 + 2 * 3))
来源：http://sqe.nwbrower.top

[R28] 浮点运算
来源：http://xaw.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://ckz.shuidangran.top

[R29] 定义函数
来源：http://bon.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yjt.yongpay.top

[R30] 函数返回状态码
来源：http://iej.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://ufd.cdnleiting.top

[R31] 局部变量
来源：http://wnb.sxryk.cn

f() { local x=1; echo "$x"; }
来源：http://qnm.316326.xyz

[R32] 参数个数校验
来源：http://xld.andypj.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ycp.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://agg.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://upv.iojbl.cn

[R34] 退出时清理
来源：http://wdu.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://shx.316326.xyz

[R35] 后台执行并等待
来源：http://ned.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://twn.fehbvm.com

[R36] 并发执行多个任务
来源：http://qco.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zal.guowangkeji.top

[R37] 把输出赋给变量
来源：http://fjm.ydjk.org.cn

files=$(ls -1)
来源：http://ctt.yonumen.top

[R38] 管道串联
来源：http://yep.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://mkl.zycfv.cn

[R39] 重定向标准输出与错误
来源：http://vvf.yuxming.cn

cmd > out.log 2>&1
来源：http://eog.chenlongwang.top

[R40] 追加写日志
来源：http://nhx.ydzc1.top

echo "log" >> out.log
来源：http://fuo.jiagoushi.top

[R41] 丢弃输出
来源：http://bjt.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://hwt.hnxiangtu.top

[R42] 输入重定向
来源：http://qae.mhx1999.top

wc -l < a.txt
来源：http://gda.xuanzx.com

[R43] 按名字查找文件
来源：http://pcq.316326.xyz

find . -name "*.log" -type f
来源：http://wll.yj20258.top

[R44] 按修改时间查找
来源：http://uof.vqdsnc.cn

find . -mtime -7 -type f
来源：http://szr.hnxiangtu.top

[R45] 批量删除
来源：http://agq.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://kgc.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://pmx.dashuyun.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ree.cashguo.top

[R47] sed 单行替换
来源：http://bgu.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://kyq.shuidangran.top

[R48] awk 取指定列
来源：http://cpa.shangyingyoupin.top

awk '{print $1, $3}' a.txt
来源：http://sdn.xziqi.cn

[R49] awk 带条件
来源：http://lfn.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xep.jqgufenzy.top

[R50] awk 求和
来源：http://uuk.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://fvh.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://qom.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gvd.xylfe.cn

[R52] 统计行数
来源：http://vuk.mhx1999.top

wc -l a.txt
来源：http://hus.dianchejie.cn

[R53] 查看文件头与实时尾
来源：http://avc.jinghuilouyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://atk.hongshengwenyu.top

[R54] 比较两个文件
来源：http://gtl.havefunace.top

diff a.txt b.txt
来源：http://toy.shuidangran.top

[R55] 压缩与解压
来源：http://oek.0kj1m.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vqg.zhoulong.xyz

[R56] 远程拷贝
来源：http://wst.ppjwa.cn

scp file user@host:/path/
来源：http://ypk.kuanghao11.cn

[R57] 远程执行命令
来源：http://bsj.snrcjt.cn

ssh user@host 'uptime'
来源：http://wyt.daxiang520.top

[R58] 下载文件
来源：http://thj.ctjpmb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rzz.yangfankeji.com

[R59] 发 POST JSON
来源：http://rxd.xingfuxueyuan.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kzw.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://sms.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yly.vehdjk.com

[R61] 磁盘占用
来源：http://fcn.guowangkeji.top

df -h;  du -sh *
来源：http://ovu.jiagoushi.top

[R62] 找最占空间的文件
来源：http://sba.bbcook.cn

du -ah . | sort -rh | head -10
来源：http://owj.zhongyouzk.top

[R63] 内存与进程
来源：http://vgw.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://wqa.9152youxi.cn

[R64] 结束进程
来源：http://olb.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://pjd.zhengqikj.top

[R65] 查看端口占用
来源：http://jtk.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://msq.shzxlz.cn

[R66] 定时任务
来源：http://ffy.0kj1m.cn

crontab -e;  crontab -l
来源：http://tmk.tarul.cn

[R67] 生成随机十六进制串
来源：http://epv.wangdashe.top

openssl rand -hex 16
来源：http://qlr.bbcook.cn

[R68] 计算文件校验值
来源：http://gqr.cdnleiting.top

sha256sum a.txt;  md5sum a.txt
来源：http://fvi.fehbvm.com

[R69] 生成随机密码
来源：http://ijc.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://hrl.ydjk.org.cn

[R70] 时间戳与互转
来源：http://ewg.quarkkingdee.top

date +%s;  date -d @1700000000
来源：http://xzw.sjlbkw.cn

[R71] 日期格式化
来源：http://bse.snrcjt.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tdg.fehbvm.com

[R72] 等待端口就绪
来源：http://hlh.nanxuanxn.top

until nc -z localhost 3306; do sleep 1; done
来源：http://giy.tian-w.cn

[R73] 分割大日志
来源：http://kgn.sweek.top

split -l 1000 big.log part_
来源：http://cvs.jiagoushi.top

[R74] 批量重命名
来源：http://uxr.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://krj.bbcook.cn

[R75] 导出环境变量
来源：http://rku.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://gpv.ppjwa.cn

[R76] 使用临时文件
来源：http://gwz.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iij.jinqigufen.top

[R77] 读取用户输入
来源：http://gyk.sysykeji.top

read -rp "请输入: " ans
来源：http://awe.sysykeji.top

[R78] 交互式菜单
来源：http://yxe.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://meu.smart0.xyz

[R79] 解析命令行选项
来源：http://pmx.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qds.yuanzhike.top

[R80] 查看脚本执行耗时
来源：http://xua.52xcode.cn

time ./run.sh
来源：http://uys.gzhubu.top

================================================================================
来源：http://nnm.jinghuilouyu.cn

S. C / C++ 专题
来源：http://utk.sweek.top

================================================================================
来源：http://rhc.cdnleiting.top

[S01] C：Hello World
来源：http://gyv.ivvv.top

#include <stdio.h>
来源：http://mkp.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qqf.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://ymn.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://xco.tianlin.xyz

[S03] C：读入整数
来源：http://mfi.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://ahw.uphjek.com

[S04] C：字符串复制
来源：http://pjv.zhijiandao.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zmk.yanxiufei.cn

[S05] C：字符串长度
来源：http://bgv.pycfn.com

strlen(s)
来源：http://qwx.shzxlz.cn

[S06] C：字符串比较
来源：http://wwl.hfpthk.cn

strcmp(a, b) == 0
来源：http://gwt.vqdsnc.cn

[S07] C：数组遍历求和
来源：http://vho.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://etd.xingfuxueyuan.xyz

[S08] C：动态内存分配与释放
来源：http://flt.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://usg.cashguo.top

[S09] C：结构体定义与初始化
来源：http://nzr.shzxlz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ong.c1oappe.top

[S10] C：指针与解引用
来源：http://wvo.nwbrower.top

int *p = &a;  *p = 5;
来源：http://uxp.ywan-chungtsiang.top

[S11] C：逐行读文件
来源：http://lgf.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://mxu.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vkf.gotoacloud.top

fclose(f);
来源：http://gxe.daxiang520.top

[S12] C：写文件
来源：http://mwl.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kxs.wangdashe.top

[S13] C：宏定义
来源：http://arq.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dzj.yanxiufei.cn

[S14] C：枚举
来源：http://ojw.hammf.cn

enum Color { RED, GREEN, BLUE };
来源：http://eah.yuanzhike.top

[S15] C：类型转换
来源：http://ztq.tian-w.cn

(double) a / b
来源：http://fdo.c1oappe.top

[S16] C：位操作置位
来源：http://dzw.0kj1m.cn

x |= (1 << 3);
来源：http://pzb.svipenyu.cn

[S17] C：安全拼接字符串
来源：http://vkp.pengpengdd.cyou

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jhs.uphjek.com

[S18] C：命令行参数
来源：http://gcd.tarul.cn

int main(int argc, char **argv)
来源：http://fbe.yj202588.top

[S19] C：快速排序
来源：http://ron.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://fkp.chenzaomai.com

[S20] C：二分查找
来源：http://fqw.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hnh.aizwys.cn

[S21] C：字符类别判断
来源：http://xrk.fzhhl.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wsa.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://rap.jqgfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://qhf.hnqzz.top

[S23] C：随机数
来源：http://xit.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jda.pengpengdd.cyou

[S24] C：获取本地时间
来源：http://sgt.zhijiandao.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://faf.jiagoushi.top

[S25] C：内存拷贝
来源：http://szg.yanxiufei.cn

memcpy(dst, src, n);
来源：http://qha.haohaochexian.top

[S26] C：内存清零
来源：http://fkw.bbcook.cn

memset(a, 0, sizeof a);
来源：http://ffq.hnxiangtu.top

[S27] C：定义常量
来源：http://ytz.zhongyouzk.top

const double PI = 3.14159;
来源：http://weo.zycfv.cn

[S28] C：静态变量
来源：http://dbj.wangdashe.top

static int counter = 0;
来源：http://igp.yfazqb.com

[S29] C：变参函数
来源：http://cak.tarul.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://isz.iojbl.cn

[S30] C：头文件保护
来源：http://ugm.cucudq.cn

#ifndef X_H
来源：http://sfe.birdmap.top

#define X_H
来源：http://odw.shuidangran.top

#endif
来源：http://mpe.zhoulong.xyz

[S31] C++：Hello World
来源：http://tna.xylfe.cn

#include <iostream>
来源：http://lir.yuanzhike.top

int main() { std::cout << "Hello\n"; }
来源：http://ryi.fzhhl.top

[S32] C++：字符串
来源：http://hut.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://vov.jqgfzy.top

[S33] C++：vector 增删
来源：http://dnq.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://whg.dashuyun.cn

[S34] C++：遍历 vector
来源：http://cdv.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://hvy.sufxvd.cn

[S35] C++：map
来源：http://gtx.pycfn.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://caa.daria6918.cn

[S36] C++：unordered_map
来源：http://flg.ybcxt.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fxy.yangfankeji.com

[S37] C++：set
来源：http://pqn.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ndz.zhaomingkeji.xyz

[S38] C++：排序
来源：http://qfv.0kj1m.cn

std::sort(v.begin(), v.end());
来源：http://tbc.pycfn.com

[S39] C++：自定义比较器排序
来源：http://mcq.xylfe.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uma.jinyuanbaomall.cn

[S40] C++：查找元素
来源：http://vvg.yj202588.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ecx.zhengqikj.top

[S41] C++：类与构造函数
来源：http://rnp.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wnk.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://wgj.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://oup.fzhhl.top

[S43] C++：智能指针
来源：http://hxo.pengpengdd.cyou

auto p = std::make_unique<int>(5);
来源：http://ovh.zhiwuduotai.top

[S44] C++：引用传参
来源：http://zov.cqqwz.cn

void inc(int &x) { ++x; }
来源：http://png.gotoacloud.top

[S45] C++：lambda
来源：http://fao.cashguo.top

auto add = [](int a, int b) { return a + b; };
来源：http://ngi.hammf.cn

[S46] C++：函数模板
来源：http://ibm.guannengcc.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ezc.sweek.top

[S47] C++：结构化绑定遍历
来源：http://zht.shanyushiyangtech.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pue.52xcode.cn

[S48] C++：逐行读文件
来源：http://vjg.cdnleiting.top

std::ifstream in("a.txt");  std::string line;
来源：http://icj.yongpay.top

while (std::getline(in, line)) { }
来源：http://doy.gzhubu.top

[S49] C++：写文件
来源：http://ccx.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zbv.jqgfzy.top

[S50] C++：格式化数字
来源：http://sod.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tvf.hongshengwenyu.top

[S51] C++：显式类型转换
来源：http://nhg.gzhubu.top

static_cast<double>(a) / b
来源：http://erf.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://rkl.wangshuangyany.cn

int size() const noexcept { return n_; }
来源：http://jxb.nwbrower.top

[S53] C++：移动语义
来源：http://fiz.jqgfzy.top

std::vector<int> w = std::move(v);
来源：http://zkd.ybcxt.top

[S54] C++：异常处理
来源：http://fis.ydjk.org.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://prg.shuidangran.top

[S55] C++：结构化绑定
来源：http://noa.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jda.zhixingplan.top

[S56] C++：optional
来源：http://igu.feifeiyinyue.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wbp.sxryk.cn

[S57] C++：编译期常量
来源：http://bda.cqqwz.cn

constexpr int N = 10;
来源：http://lih.yj20258888.top

[S58] C++：命名空间
来源：http://put.jinghuilouyu.cn

namespace ns { int f() { return 1; } }
来源：http://vwv.havefunace.top

[S59] C++：静态断言
来源：http://hdz.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ndb.sxryk.cn

[S60] C++：遍历并删除元素
来源：http://mfr.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://txd.guannengcc.top

================================================================================
来源：http://qpr.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aci.hnqzz.top

================================================================================
来源：http://msf.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://zeb.yongpay.top

println("Hello")
来源：http://jnx.yongpay.top

[T02] Kotlin：变量
来源：http://pdt.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eep.yj202588.top

[T03] Kotlin：字符串模板
来源：http://iuo.jyoumei.cn

"值: $b"
来源：http://yzy.jiagoushi.top

[T04] Kotlin：空安全
来源：http://wji.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://wxr.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://jkf.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hyn.chenjidiqi.icu

[T06] Kotlin：集合映射
来源：http://ohs.fzhhl.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hii.sweek.top

[T07] Kotlin：集合过滤
来源：http://gqa.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sdr.yj20258888.top

[T08] Kotlin：数据类
来源：http://vub.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://emh.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://rfn.yonumen.top

fun String.exclaim() = this + "!"
来源：http://tqw.yj20258.top

[T10] Kotlin：默认参数
来源：http://mhi.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kty.zhixingplan.top

[T11] Kotlin：协程
来源：http://anu.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hfv.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://ukg.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://beh.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://olc.fktsv.cn

val m = mapOf("a" to 1)
来源：http://fkb.ivvv.top

[T14] Kotlin：循环
来源：http://bkm.cqqwz.cn

for (i in 1..10) println(i)
来源：http://jfr.shanyushiyangkeji.top


<!-- 参考信息 -->