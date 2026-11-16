代发 wailian999

esac
来源：http://tam.guannengcc.top

[R12] for 遍历文件
来源：http://poz.shuidangran.top

for f in *.txt; do echo "$f"; done
来源：http://lqu.yonumen.top

[R13] for 计数循环
来源：http://jek.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://rxq.shangyingyoupin.top

[R14] C 风格 for
来源：http://pou.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oyp.jqgfzy.top

[R15] while 逐行读文件
来源：http://tog.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hbw.kuanghao11.cn

[R16] until 等待条件
来源：http://tsr.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uzq.kuanghao11.cn

[R17] 数组定义与取值
来源：http://vzj.aibaodan.cn

arr=(a b c); echo "${arr[0]}"
来源：http://azq.zhijiandao.cn

[R18] 遍历数组
来源：http://vjo.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vmq.jyoumei.cn

[R19] 数组长度
来源：http://wrk.gotoacloud.top

echo "${#arr[@]}"
来源：http://fry.havefunace.top

[R20] 关联数组（字典）
来源：http://hhw.shzxlz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eai.hongshengwenyu.top

[R21] 字符串长度
来源：http://pxh.52xcode.cn

echo "${#s}"
来源：http://zbs.xziqi.cn

[R22] 截取子串
来源：http://rxv.wangdashe.top

echo "${s:0:5}"
来源：http://pgd.yj20258.top

[R23] 字符串替换
来源：http://aqk.chenlongwang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gss.yuanzhike.top

[R24] 大小写转换
来源：http://rfl.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://ykz.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://bgz.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://zry.zhongyouzk.top

[R26] 命令替换
来源：http://gsk.zhengqikj.top

now=$(date +%F); echo "$now"
来源：http://vzd.fehbvm.com

[R27] 算术展开
来源：http://mxj.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://npb.52xcode.cn

[R28] 浮点运算
来源：http://daf.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://mmk.hnqzz.top

[R29] 定义函数
来源：http://iyd.zhengqikj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hop.epnwcf.com

[R30] 函数返回状态码
来源：http://dus.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://bcl.zhijiandao.cn

[R31] 局部变量
来源：http://rzs.haohaochexian.top

f() { local x=1; echo "$x"; }
来源：http://zvf.zdbjq.cn

[R32] 参数个数校验
来源：http://nif.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gxj.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://keg.yj20258.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://srf.xziqi.cn

[R34] 退出时清理
来源：http://gmh.dianchejie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sca.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://wsa.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zii.yangfankeji.com

[R36] 并发执行多个任务
来源：http://fek.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hph.nanxuanxn.top

[R37] 把输出赋给变量
来源：http://pwy.nanxuanxn.top

files=$(ls -1)
来源：http://tqx.sjlbkw.cn

[R38] 管道串联
来源：http://bju.tianlin.xyz

cat a.txt | grep -i error | wc -l
来源：http://xqw.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://xen.aibaodan.cn

cmd > out.log 2>&1
来源：http://iky.zhongyouzk.top

[R40] 追加写日志
来源：http://dck.smart0.xyz

echo "log" >> out.log
来源：http://iiv.gotoacloud.top

[R41] 丢弃输出
来源：http://kwr.hywenlv.cn

cmd >/dev/null 2>&1
来源：http://uyv.hnqzz.top

[R42] 输入重定向
来源：http://kwg.iojbl.cn

wc -l < a.txt
来源：http://yzh.tian-w.cn

[R43] 按名字查找文件
来源：http://yuo.yuxming.cn

find . -name "*.log" -type f
来源：http://jdm.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://qjq.xuanzx.com

find . -mtime -7 -type f
来源：http://cuv.pycfn.com

[R45] 批量删除
来源：http://ysf.aibaodan.cn

find . -name "*.tmp" -delete
来源：http://jro.zhaomingkeji.xyz

[R46] 递归替换文件内容
来源：http://kzz.tianlin.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://moe.c1oappe.top

[R47] sed 单行替换
来源：http://esp.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://gcg.316326.xyz

[R48] awk 取指定列
来源：http://tpv.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://ouf.shangyingyoupin.top

[R49] awk 带条件
来源：http://qlx.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://les.cqqwz.cn

[R50] awk 求和
来源：http://ljk.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://bmz.0kj1m.cn

[R51] 排序去重取前几
来源：http://obv.nanxuanxn.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pck.ppjwa.cn

[R52] 统计行数
来源：http://sjo.nanxuanxn.top

wc -l a.txt
来源：http://fmu.guowangkeji.top

[R53] 查看文件头与实时尾
来源：http://guj.hfpthk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://acg.zhixingplan.top

[R54] 比较两个文件
来源：http://oks.c1oappe.top

diff a.txt b.txt
来源：http://zzq.jinqigufen.top

[R55] 压缩与解压
来源：http://qdb.birdmap.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jhm.chenjidiqi.icu

[R56] 远程拷贝
来源：http://wgr.nanxinkj.top

scp file user@host:/path/
来源：http://opw.pycfn.com

[R57] 远程执行命令
来源：http://sue.ydzc1.top

ssh user@host 'uptime'
来源：http://kvi.birdmap.top

[R58] 下载文件
来源：http://lfw.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pdb.jinqigufen.top

[R59] 发 POST JSON
来源：http://eer.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://glo.ybcxt.top

[R60] 只看 HTTP 状态码
来源：http://bqc.snrcjt.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jkc.xuetiantiany.cn

[R61] 磁盘占用
来源：http://doo.yj20258888.top

df -h;  du -sh *
来源：http://whn.ydzc1.top

[R62] 找最占空间的文件
来源：http://azv.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://aps.zycfv.cn

[R63] 内存与进程
来源：http://nmd.hywenlv.cn

free -h;  ps aux | grep nginx
来源：http://jsy.tian-w.cn

[R64] 结束进程
来源：http://ulq.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://mpm.yangfankeji.com

[R65] 查看端口占用
来源：http://hoi.yvedp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://upx.nanxinkj.top

[R66] 定时任务
来源：http://gkn.wangdashe.top

crontab -e;  crontab -l
来源：http://ghq.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://cap.redwolf501.top

openssl rand -hex 16
来源：http://hho.yanxiufei.cn

[R68] 计算文件校验值
来源：http://jpw.sweek.top

sha256sum a.txt;  md5sum a.txt
来源：http://wrn.svipenyu.cn

[R69] 生成随机密码
来源：http://vkl.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://acb.birdmap.top

[R70] 时间戳与互转
来源：http://jbw.jinqigufen.top

date +%s;  date -d @1700000000
来源：http://hrw.hongshengwenyu.top

[R71] 日期格式化
来源：http://fut.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zku.wangdashe.top

[R72] 等待端口就绪
来源：http://vdx.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vtv.redwolf501.top

[R73] 分割大日志
来源：http://hjv.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://dcd.tarul.cn

[R74] 批量重命名
来源：http://yom.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rzb.nanxinkj.top

[R75] 导出环境变量
来源：http://wro.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://jgh.daria6918.cn

[R76] 使用临时文件
来源：http://crk.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fij.zhongyouzk.top

[R77] 读取用户输入
来源：http://jjd.zhengqikj.top

read -rp "请输入: " ans
来源：http://tho.yuanzhike.top

[R78] 交互式菜单
来源：http://ukv.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ins.hcnkem.com

[R79] 解析命令行选项
来源：http://wnw.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jse.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://vro.daxiang520.top

time ./run.sh
来源：http://bzp.andypj.xyz

================================================================================
来源：http://wxe.vqdsnc.cn

S. C / C++ 专题
来源：http://fyl.zhiwuduotai.top

================================================================================
来源：http://tqm.ybcxt.top

[S01] C：Hello World
来源：http://ncv.yuanzhike.top

#include <stdio.h>
来源：http://qgo.sufxvd.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tta.daxiang520.top

[S02] C：变量与格式化输出
来源：http://apf.gotoacloud.top

int a = 10; printf("%d\n", a);
来源：http://vvn.sufxvd.cn

[S03] C：读入整数
来源：http://mmq.xuanzx.com

int x; scanf("%d", &x);
来源：http://rdx.bjfxy.top

[S04] C：字符串复制
来源：http://rav.haohaochexian.top

char dst[32]; strcpy(dst, "hi");
来源：http://svj.zhijiandao.cn

[S05] C：字符串长度
来源：http://vwn.snrcjt.cn

strlen(s)
来源：http://maf.jinqigufen.top

[S06] C：字符串比较
来源：http://fkz.nanxinkj.top

strcmp(a, b) == 0
来源：http://wdh.iojbl.cn

[S07] C：数组遍历求和
来源：http://yot.hcnkem.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lps.pycfn.com

[S08] C：动态内存分配与释放
来源：http://pts.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://laz.fanxiaobao.xyz

[S09] C：结构体定义与初始化
来源：http://tob.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tof.ivvv.top

[S10] C：指针与解引用
来源：http://mws.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://rlc.zhixingplan.top

[S11] C：逐行读文件
来源：http://rxn.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://vpa.hnxiangtu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vny.zhijiandao.cn

fclose(f);
来源：http://pgm.ywan-chungtsiang.top

[S12] C：写文件
来源：http://tpk.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mzh.hammf.cn

[S13] C：宏定义
来源：http://cmj.gaohongyu789.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kit.zhijiandao.cn

[S14] C：枚举
来源：http://bpf.jinqigfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://tmm.jyoumei.cn

[S15] C：类型转换
来源：http://cdi.guowangkeji.top

(double) a / b
来源：http://eop.jinqigfzy.top

[S16] C：位操作置位
来源：http://czj.dianchejie.cn

x |= (1 << 3);
来源：http://ath.jinyuanbaomall.cn

[S17] C：安全拼接字符串
来源：http://ccl.sweek.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dgk.ydjk.org.cn

[S18] C：命令行参数
来源：http://obr.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://kep.ybcxt.top

[S19] C：快速排序
来源：http://mdp.hongshengwenyu.top

qsort(a, n, sizeof(int), cmp);
来源：http://prw.yueranfly.top

[S20] C：二分查找
来源：http://zat.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wuo.gogol.net.cn

[S21] C：字符类别判断
来源：http://wmo.svipenyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hgq.fehbvm.com

[S22] C：字符串转数字
来源：http://onb.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://xjs.tarul.cn

[S23] C：随机数
来源：http://whu.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kbw.shuidangran.top

[S24] C：获取本地时间
来源：http://bgs.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://igj.bbcook.cn

[S25] C：内存拷贝
来源：http://kjg.yj202588.top

memcpy(dst, src, n);
来源：http://qqx.hysaishi.cn

[S26] C：内存清零
来源：http://hck.jlsjyb.cn

memset(a, 0, sizeof a);
来源：http://dgd.hnxiangtu.top

[S27] C：定义常量
来源：http://fhl.jianghu66.top

const double PI = 3.14159;
来源：http://kdm.meibo888.top

[S28] C：静态变量
来源：http://mlp.aibaodan.cn

static int counter = 0;
来源：http://fio.aibaodan.cn

[S29] C：变参函数
来源：http://haq.tanke756.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sda.daria6918.cn

[S30] C：头文件保护
来源：http://rcr.quarkkingdee.top

#ifndef X_H
来源：http://was.hnqzz.top

#define X_H
来源：http://mqh.ehwqpu.com

#endif
来源：http://fys.iojbl.cn

[S31] C++：Hello World
来源：http://pkw.hysaishi.cn

#include <iostream>
来源：http://vce.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://cnn.ybcxt.top

[S32] C++：字符串
来源：http://swy.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://ycd.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://jif.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zrc.jqgfzy.top

[S34] C++：遍历 vector
来源：http://abf.ydzc1.top

for (auto &x : v) { std::cout << x; }
来源：http://iui.havefunace.top

[S35] C++：map
来源：http://kli.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bei.hysaishi.cn

[S36] C++：unordered_map
来源：http://ygq.sufxvd.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gxr.mhx1999.top

[S37] C++：set
来源：http://sso.hesvh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wpu.shanyushiyangtech.top

[S38] C++：排序
来源：http://khf.tarul.cn

std::sort(v.begin(), v.end());
来源：http://fal.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://dvg.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aui.xylfe.cn

[S40] C++：查找元素
来源：http://ldr.iojbl.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gha.wangdashe.top

[S41] C++：类与构造函数
来源：http://hzg.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://utw.c1oappe.top

[S42] C++：继承与虚函数
来源：http://qvn.sufxvd.cn

class B : public Base { public: void f() override {} };
来源：http://hww.shuidangran.top

[S43] C++：智能指针
来源：http://zju.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://ttu.zhaomingkeji.xyz

[S44] C++：引用传参
来源：http://ssc.havefunace.top

void inc(int &x) { ++x; }
来源：http://tho.bjfxy.top

[S45] C++：lambda
来源：http://hfy.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://qvk.hcnkem.com

[S46] C++：函数模板
来源：http://bvf.zhijiandao.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nys.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://qec.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mwg.yj202588.top

[S48] C++：逐行读文件
来源：http://kpi.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cag.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://yzi.haohaochexian.top

[S49] C++：写文件
来源：http://ocx.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ryd.vqdsnc.cn

[S50] C++：格式化数字
来源：http://imv.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fmb.c1oappe.top

[S51] C++：显式类型转换
来源：http://onf.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://jtj.ywan-chungtsiang.top

[S52] C++：const 与 noexcept
来源：http://pua.daxiang520.top

int size() const noexcept { return n_; }
来源：http://qpb.zdbjq.cn

[S53] C++：移动语义
来源：http://gry.jinghuilouyu.cn

std::vector<int> w = std::move(v);
来源：http://aio.yonumen.top

[S54] C++：异常处理
来源：http://qfe.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sur.zdbjq.cn

[S55] C++：结构化绑定
来源：http://xce.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mvh.jiagoushi.top

[S56] C++：optional
来源：http://woo.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kvf.svipenyu.cn

[S57] C++：编译期常量
来源：http://gsq.chenzaomai.com

constexpr int N = 10;
来源：http://nrh.andypj.xyz

[S58] C++：命名空间
来源：http://fnr.0kj1m.cn

namespace ns { int f() { return 1; } }
来源：http://ikf.316326.xyz

[S59] C++：静态断言
来源：http://oxs.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wlt.ybcxt.top

[S60] C++：遍历并删除元素
来源：http://jmz.uphjek.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zib.yanxiufei.cn

================================================================================
来源：http://qau.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://srh.fehbvm.com

================================================================================
来源：http://ntw.sweek.top

[T01] Kotlin：Hello World
来源：http://zoq.redwolf501.top

println("Hello")
来源：http://diw.nanxinkj.top

[T02] Kotlin：变量
来源：http://dqd.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gra.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://lfh.nanxinkj.top

"值: $b"
来源：http://loq.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://ufq.zhongyouzk.top

val n: String? = null;  n?.length
来源：http://sir.fengsongda.top

[T05] Kotlin：when 表达式
来源：http://xdd.zhixingplan.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qpc.tian-w.cn

[T06] Kotlin：集合映射
来源：http://kul.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://oqp.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://jvz.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://snw.sufxvd.cn

[T08] Kotlin：数据类
来源：http://okp.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://bsh.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://ldh.jinghuilouyu.cn

fun String.exclaim() = this + "!"
来源：http://ybg.shzxlz.cn

[T10] Kotlin：默认参数
来源：http://xzt.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://oci.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://iyv.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ojz.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://bzn.smart0.xyz

val (a, b) = Pair(1, 2)
来源：http://kss.uphjek.com

[T13] Kotlin：只读 Map
来源：http://lqo.hnxiangtu.top

val m = mapOf("a" to 1)
来源：http://ehi.wangdashe.top

[T14] Kotlin：循环
来源：http://rpz.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://wnm.nwbrower.top


<!-- 参考信息 -->