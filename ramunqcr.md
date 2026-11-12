代发 wailian999

esac
来源：http://cwt.nwbrower.top

[R12] for 遍历文件
来源：http://eds.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://vui.zhijiandao.cn

[R13] for 计数循环
来源：http://xns.chenlongwang.top

for i in {1..10}; do echo "$i"; done
来源：http://kdb.cashguo.top

[R14] C 风格 for
来源：http://ddu.zycfv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nsm.wangdashe.top

[R15] while 逐行读文件
来源：http://zpj.xuanzx.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dlo.hfpthk.cn

[R16] until 等待条件
来源：http://hhy.aibaodan.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fwx.zhengqikj.top

[R17] 数组定义与取值
来源：http://ndw.wangshuangyany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://teq.ywan-chungtsiang.top

[R18] 遍历数组
来源：http://qnn.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rck.andypj.xyz

[R19] 数组长度
来源：http://vra.zhengqikj.top

echo "${#arr[@]}"
来源：http://wyg.fehbvm.com

[R20] 关联数组（字典）
来源：http://tni.zhixingplan.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cxz.shzxlz.cn

[R21] 字符串长度
来源：http://zcy.yueranfly.top

echo "${#s}"
来源：http://skw.jiagoushi.top

[R22] 截取子串
来源：http://wkk.fengsongda.top

echo "${s:0:5}"
来源：http://odi.tianlin.xyz

[R23] 字符串替换
来源：http://xhm.daria6918.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cnt.sufxvd.cn

[R24] 大小写转换
来源：http://mpp.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nbr.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://exv.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://dnj.chenzaomai.com

[R26] 命令替换
来源：http://enf.cheryme.top

now=$(date +%F); echo "$now"
来源：http://uaz.xuetiantiany.cn

[R27] 算术展开
来源：http://fgc.yj20258888.top

echo $((1 + 2 * 3))
来源：http://hse.gzhubu.top

[R28] 浮点运算
来源：http://zpf.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://fok.gotoacloud.top

[R29] 定义函数
来源：http://los.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rmp.ehwqpu.com

[R30] 函数返回状态码
来源：http://hgi.yj20258888.top

f() { return 0; }; f || echo "失败了"
来源：http://nvk.zhiwuduotai.top

[R31] 局部变量
来源：http://lqn.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://usz.zhongyouzk.top

[R32] 参数个数校验
来源：http://hvt.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://suj.gaohongyu789.top

[R33] 捕获错误并提示行号
来源：http://wbq.xingfuxueyuan.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yhb.xinyue.icu

[R34] 退出时清理
来源：http://eia.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://rky.yanxiufei.cn

[R35] 后台执行并等待
来源：http://yra.dianchejie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rfe.cucudq.cn

[R36] 并发执行多个任务
来源：http://qvg.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ozo.birdmap.top

[R37] 把输出赋给变量
来源：http://pha.ehwqpu.com

files=$(ls -1)
来源：http://svo.vqdsnc.cn

[R38] 管道串联
来源：http://nyb.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://ayi.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://vut.vqdsnc.cn

cmd > out.log 2>&1
来源：http://msn.52xcode.cn

[R40] 追加写日志
来源：http://kyb.yuxming.cn

echo "log" >> out.log
来源：http://spf.feifeiyinyue.top

[R41] 丢弃输出
来源：http://oqp.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://edv.yangfankeji.com

[R42] 输入重定向
来源：http://fmy.hammf.cn

wc -l < a.txt
来源：http://fop.jlsjyb.cn

[R43] 按名字查找文件
来源：http://hnc.xingfuxueyuan.xyz

find . -name "*.log" -type f
来源：http://vob.sjlbkw.cn

[R44] 按修改时间查找
来源：http://sec.snrcjt.cn

find . -mtime -7 -type f
来源：http://zom.vehdjk.com

[R45] 批量删除
来源：http://xad.0kj1m.cn

find . -name "*.tmp" -delete
来源：http://oxv.cucudq.cn

[R46] 递归替换文件内容
来源：http://ssi.sufxvd.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rfj.cashguo.top

[R47] sed 单行替换
来源：http://tny.tanke756.top

sed -i 's/foo/bar/g' a.txt
来源：http://rvx.hnxiangtu.top

[R48] awk 取指定列
来源：http://xyg.ydjk.org.cn

awk '{print $1, $3}' a.txt
来源：http://foh.tanke756.top

[R49] awk 带条件
来源：http://oys.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ddr.gaohongyu789.top

[R50] awk 求和
来源：http://vda.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://gun.aizwys.cn

[R51] 排序去重取前几
来源：http://oye.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vsp.hywenlv.cn

[R52] 统计行数
来源：http://wjp.yfazqb.com

wc -l a.txt
来源：http://czb.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://byl.sysykeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://esm.jiagoushi.top

[R54] 比较两个文件
来源：http://rwz.yuanzhike.top

diff a.txt b.txt
来源：http://hnq.nwbrower.top

[R55] 压缩与解压
来源：http://kye.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mlw.yuanzhike.top

[R56] 远程拷贝
来源：http://vwj.jqgfzy.top

scp file user@host:/path/
来源：http://jrw.shanyushiyangkeji.top

[R57] 远程执行命令
来源：http://bzt.redwolf501.top

ssh user@host 'uptime'
来源：http://vqt.chenlongwang.top

[R58] 下载文件
来源：http://pra.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xxp.vqdsnc.cn

[R59] 发 POST JSON
来源：http://fao.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mgu.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://hvs.yanxiufei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ilm.andypj.xyz

[R61] 磁盘占用
来源：http://irg.zhongyouzk.top

df -h;  du -sh *
来源：http://kgc.jinqigfzy.top

[R62] 找最占空间的文件
来源：http://fzg.uphjek.com

du -ah . | sort -rh | head -10
来源：http://kyf.fzhhl.top

[R63] 内存与进程
来源：http://tig.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://neh.gaohongyu789.top

[R64] 结束进程
来源：http://vbq.ehwqpu.com

kill -9 $(pgrep -f app.py)
来源：http://xpg.yuxming.cn

[R65] 查看端口占用
来源：http://ffw.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vpa.gotoacloud.top

[R66] 定时任务
来源：http://cbr.fengsongda.top

crontab -e;  crontab -l
来源：http://xvd.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://zzk.zhixingplan.top

openssl rand -hex 16
来源：http://kjt.pengpengdd.cyou

[R68] 计算文件校验值
来源：http://shd.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://ikj.gaohongyu789.top

[R69] 生成随机密码
来源：http://ftz.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://alg.ehwqpu.com

[R70] 时间戳与互转
来源：http://yrh.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://rqp.shanyushiyangtech.top

[R71] 日期格式化
来源：http://xvi.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://woy.svipenyu.cn

[R72] 等待端口就绪
来源：http://nbl.yj20258888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cym.chenzaomai.com

[R73] 分割大日志
来源：http://duv.hnqzz.top

split -l 1000 big.log part_
来源：http://axl.jinqigufen.top

[R74] 批量重命名
来源：http://bxh.zycfv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://diy.jianghu66.top

[R75] 导出环境变量
来源：http://zfq.xingfuxueyuan.xyz

export PATH="$HOME/bin:$PATH"
来源：http://zwy.wangshuangyany.cn

[R76] 使用临时文件
来源：http://cpr.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://axf.yueranfly.top

[R77] 读取用户输入
来源：http://suk.guannengcc.top

read -rp "请输入: " ans
来源：http://mng.sweek.top

[R78] 交互式菜单
来源：http://crd.fehbvm.com

select opt in a b c; do echo "$opt"; break; done
来源：http://puo.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://apm.c1oappe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gmf.tianlin.xyz

[R80] 查看脚本执行耗时
来源：http://myt.gotoacloud.top

time ./run.sh
来源：http://zjr.snrcjt.cn

================================================================================
来源：http://jts.yfazqb.com

S. C / C++ 专题
来源：http://wgb.fehbvm.com

================================================================================
来源：http://tds.hysaishi.cn

[S01] C：Hello World
来源：http://kah.chenlongwang.top

#include <stdio.h>
来源：http://lqe.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://evk.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://emb.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://dgq.jqgfzy.top

[S03] C：读入整数
来源：http://cnl.xinyue.icu

int x; scanf("%d", &x);
来源：http://brx.xylfe.cn

[S04] C：字符串复制
来源：http://vxh.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://flc.ppjwa.cn

[S05] C：字符串长度
来源：http://zpa.hongshengwenyu.top

strlen(s)
来源：http://gwf.yonumen.top

[S06] C：字符串比较
来源：http://xto.nanxuanxn.top

strcmp(a, b) == 0
来源：http://aow.fzhhl.top

[S07] C：数组遍历求和
来源：http://wpg.wangdashe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rmx.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://tdj.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cav.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://hpl.nwbrower.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://inm.hnxiangtu.top

[S10] C：指针与解引用
来源：http://mlp.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://tmk.guannengcc.top

[S11] C：逐行读文件
来源：http://uzj.jqgfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://ulo.jlsjyb.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://usw.tianlin.xyz

fclose(f);
来源：http://aou.haohaochexian.top

[S12] C：写文件
来源：http://tsh.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rbh.chenjidiqi.icu

[S13] C：宏定义
来源：http://klr.xingfuxueyuan.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bom.mhx1999.top

[S14] C：枚举
来源：http://gem.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://idm.jlsjyb.cn

[S15] C：类型转换
来源：http://uzr.jqgfzy.top

(double) a / b
来源：http://xei.cucudq.cn

[S16] C：位操作置位
来源：http://zbs.gzhubu.top

x |= (1 << 3);
来源：http://dfg.tarul.cn

[S17] C：安全拼接字符串
来源：http://cek.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ymy.chenjidiqi.icu

[S18] C：命令行参数
来源：http://nfs.ctjpmb.com

int main(int argc, char **argv)
来源：http://kfm.fzhhl.top

[S19] C：快速排序
来源：http://rbg.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://pkj.jinqigfzy.top

[S20] C：二分查找
来源：http://gmk.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://esn.guowangkeji.top

[S21] C：字符类别判断
来源：http://kvm.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aog.zhoulong.xyz

[S22] C：字符串转数字
来源：http://ims.fengsongda.top

atoi("42");  strtod("3.14", NULL);
来源：http://juu.bjfxy.top

[S23] C：随机数
来源：http://sec.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://snf.zdbjq.cn

[S24] C：获取本地时间
来源：http://qbr.pengpengdd.cyou

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dyn.hammf.cn

[S25] C：内存拷贝
来源：http://rrs.tanke756.top

memcpy(dst, src, n);
来源：http://pol.vehdjk.com

[S26] C：内存清零
来源：http://srg.tian-w.cn

memset(a, 0, sizeof a);
来源：http://zsl.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://znm.yj20258888.top

const double PI = 3.14159;
来源：http://kqz.cqqwz.cn

[S28] C：静态变量
来源：http://hbj.vehdjk.com

static int counter = 0;
来源：http://smb.pycfn.com

[S29] C：变参函数
来源：http://cqq.guannengcc.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mtv.fktsv.cn

[S30] C：头文件保护
来源：http://jsx.yongpay.top

#ifndef X_H
来源：http://xyz.kuanghao11.cn

#define X_H
来源：http://mly.quarkkingdee.top

#endif
来源：http://ltd.hesvh.cn

[S31] C++：Hello World
来源：http://dqn.birdmap.top

#include <iostream>
来源：http://okw.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://cbj.ywan-chungtsiang.top

[S32] C++：字符串
来源：http://ofq.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://yws.yongpay.top

[S33] C++：vector 增删
来源：http://ymz.hysaishi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jah.gzhubu.top

[S34] C++：遍历 vector
来源：http://emd.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://jow.dashuyun.cn

[S35] C++：map
来源：http://yca.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nnr.gogol.net.cn

[S36] C++：unordered_map
来源：http://yhc.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wmx.hammf.cn

[S37] C++：set
来源：http://cjz.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dsu.jinyuanbaomall.cn

[S38] C++：排序
来源：http://tcj.pengpengdd.cyou

std::sort(v.begin(), v.end());
来源：http://dyn.zycfv.cn

[S39] C++：自定义比较器排序
来源：http://gpd.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pcu.xuanzx.com

[S40] C++：查找元素
来源：http://bfa.aibaodan.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lzj.yj20258.top

[S41] C++：类与构造函数
来源：http://pmp.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jgy.wangdashe.top

[S42] C++：继承与虚函数
来源：http://col.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://hoo.epnwcf.com

[S43] C++：智能指针
来源：http://wyz.zhijiandao.cn

auto p = std::make_unique<int>(5);
来源：http://huq.sufxvd.cn

[S44] C++：引用传参
来源：http://gmc.sysykeji.top

void inc(int &x) { ++x; }
来源：http://uzy.pengpengdd.cyou

[S45] C++：lambda
来源：http://vnr.cdnleiting.top

auto add = [](int a, int b) { return a + b; };
来源：http://qtd.smart0.xyz

[S46] C++：函数模板
来源：http://kcp.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qgw.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://vnh.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nlj.nanxinkj.top

[S48] C++：逐行读文件
来源：http://qih.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yze.hnxiangtu.top

while (std::getline(in, line)) { }
来源：http://feo.yonumen.top

[S49] C++：写文件
来源：http://pup.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ryr.epnwcf.com

[S50] C++：格式化数字
来源：http://ado.iojbl.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kaf.316326.xyz

[S51] C++：显式类型转换
来源：http://qnd.52xcode.cn

static_cast<double>(a) / b
来源：http://wnd.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://rqq.cheryme.top

int size() const noexcept { return n_; }
来源：http://kjm.yuanzhike.top

[S53] C++：移动语义
来源：http://lvk.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://dtk.xziqi.cn

[S54] C++：异常处理
来源：http://vjy.birdmap.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dyx.ydjk.org.cn

[S55] C++：结构化绑定
来源：http://uhr.gogol.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://njh.birdmap.top

[S56] C++：optional
来源：http://agi.ybcxt.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bjl.ctjpmb.com

[S57] C++：编译期常量
来源：http://sjt.sjlbkw.cn

constexpr int N = 10;
来源：http://fbi.fengsongda.top

[S58] C++：命名空间
来源：http://inh.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://qbq.mhx1999.top

[S59] C++：静态断言
来源：http://iyn.gotoacloud.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gel.ivvv.top

[S60] C++：遍历并删除元素
来源：http://ptg.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jpb.yueranfly.top

================================================================================
来源：http://snd.tianlin.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pch.xuanzx.com

================================================================================
来源：http://oay.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://nhl.tianlin.xyz

println("Hello")
来源：http://qkc.pycfn.com

[T02] Kotlin：变量
来源：http://sfi.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dgc.havefunace.top

[T03] Kotlin：字符串模板
来源：http://hqm.yongpay.top

"值: $b"
来源：http://ixz.haohaochexian.top

[T04] Kotlin：空安全
来源：http://hto.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://xhd.fktsv.cn

[T05] Kotlin：when 表达式
来源：http://nxj.andypj.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tqz.kuanghao11.cn

[T06] Kotlin：集合映射
来源：http://reo.uphjek.com

listOf(1, 2, 3).map { it * 2 }
来源：http://cmm.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://tpf.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vom.vehdjk.com

[T08] Kotlin：数据类
来源：http://dnq.ydjk.org.cn

data class User(val name: String, val age: Int)
来源：http://dyz.havefunace.top

[T09] Kotlin：扩展函数
来源：http://est.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://sab.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://zza.yanxiufei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://snv.ybcxt.top

[T11] Kotlin：协程
来源：http://znw.jiagoushi.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fas.tanke756.top

[T12] Kotlin：解构声明
来源：http://xut.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://qok.fzhhl.top

[T13] Kotlin：只读 Map
来源：http://wao.sxryk.cn

val m = mapOf("a" to 1)
来源：http://aub.ctjpmb.com

[T14] Kotlin：循环
来源：http://thw.zhixingplan.top

for (i in 1..10) println(i)
来源：http://ezm.jinghuilouyu.cn


<!-- 参考信息 -->