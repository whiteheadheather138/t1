代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tpg.hfpthk.cn

[R10] 正则匹配
来源：http://lec.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xtx.bbcook.cn

[R11] case 多分支
来源：http://bsg.cdnleiting.top

case "$1" in
来源：http://ihz.shuidangran.top

start) echo "启动" ;;
来源：http://lds.meibo888.top

stop)  echo "停止" ;;
来源：http://lqg.zhaomingkeji.xyz

*)     echo "未知命令" ;;
来源：http://uil.yj20258888.top

esac
来源：http://tfq.0kj1m.cn

[R12] for 遍历文件
来源：http://crh.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://etz.shuidangran.top

[R13] for 计数循环
来源：http://eez.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://tuf.jinghuilouyu.cn

[R14] C 风格 for
来源：http://evp.xuetiantiany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cej.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://gzw.nanxuanxn.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://had.fzhhl.top

[R16] until 等待条件
来源：http://lpw.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ioe.52xcode.cn

[R17] 数组定义与取值
来源：http://eko.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gyl.ivvv.top

[R18] 遍历数组
来源：http://jzv.snrcjt.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hep.316326.xyz

[R19] 数组长度
来源：http://usx.svipenyu.cn

echo "${#arr[@]}"
来源：http://wfd.xingfuxueyuan.xyz

[R20] 关联数组（字典）
来源：http://gja.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://raz.ydzc1.top

[R21] 字符串长度
来源：http://hgy.sysykeji.top

echo "${#s}"
来源：http://rev.ybcxt.top

[R22] 截取子串
来源：http://mxj.xuanzx.com

echo "${s:0:5}"
来源：http://qak.wangshuangyany.cn

[R23] 字符串替换
来源：http://rhq.sysykeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xrx.52xcode.cn

[R24] 大小写转换
来源：http://xlz.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zpv.cheryme.top

[R25] 去后缀 / 去前缀
来源：http://mlp.yj20258888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kov.hcnkem.com

[R26] 命令替换
来源：http://mre.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://iby.xuanzx.com

[R27] 算术展开
来源：http://crf.yj20258.top

echo $((1 + 2 * 3))
来源：http://dav.svipenyu.cn

[R28] 浮点运算
来源：http://lug.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://bio.hfpthk.cn

[R29] 定义函数
来源：http://wgn.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cud.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://vdo.zhijiandao.cn

f() { return 0; }; f || echo "失败了"
来源：http://niv.fzhhl.top

[R31] 局部变量
来源：http://afs.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://hzj.jqgufenzy.top

[R32] 参数个数校验
来源：http://myl.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wdd.mhx1999.top

[R33] 捕获错误并提示行号
来源：http://ous.nanxuanxn.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vxc.ehwqpu.com

[R34] 退出时清理
来源：http://giz.9152youxi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yjx.jianghu66.top

[R35] 后台执行并等待
来源：http://wva.hnxiangtu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://onj.svipenyu.cn

[R36] 并发执行多个任务
来源：http://nzc.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nin.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://sbh.gaohongyu789.top

files=$(ls -1)
来源：http://uxd.jinqigufen.top

[R38] 管道串联
来源：http://ihu.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://sqs.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://zdp.iojbl.cn

cmd > out.log 2>&1
来源：http://hfo.cucudq.cn

[R40] 追加写日志
来源：http://plb.jlsjyb.cn

echo "log" >> out.log
来源：http://hcj.yanxiufei.cn

[R41] 丢弃输出
来源：http://bzz.bbcook.cn

cmd >/dev/null 2>&1
来源：http://lqq.nanxuanxn.top

[R42] 输入重定向
来源：http://imw.0kj1m.cn

wc -l < a.txt
来源：http://pvo.epnwcf.com

[R43] 按名字查找文件
来源：http://vwl.fzhhl.top

find . -name "*.log" -type f
来源：http://ucq.xingfuxueyuan.xyz

[R44] 按修改时间查找
来源：http://rum.xuanzx.com

find . -mtime -7 -type f
来源：http://tgg.sysykeji.top

[R45] 批量删除
来源：http://pci.uphjek.com

find . -name "*.tmp" -delete
来源：http://jgd.dashuyun.cn

[R46] 递归替换文件内容
来源：http://ret.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sap.birdmap.top

[R47] sed 单行替换
来源：http://vze.vehdjk.com

sed -i 's/foo/bar/g' a.txt
来源：http://syf.jyoumei.cn

[R48] awk 取指定列
来源：http://xna.quarkkingdee.top

awk '{print $1, $3}' a.txt
来源：http://pgi.tian-w.cn

[R49] awk 带条件
来源：http://vdc.yonumen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fav.fengsongda.top

[R50] awk 求和
来源：http://zdi.jlsjyb.cn

awk '{s += $2} END {print s}' a.txt
来源：http://reg.ehwqpu.com

[R51] 排序去重取前几
来源：http://xlr.iojbl.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sij.ydzc1.top

[R52] 统计行数
来源：http://vhj.xziqi.cn

wc -l a.txt
来源：http://gyk.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://swb.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://stv.hysaishi.cn

[R54] 比较两个文件
来源：http://bmm.daxiang520.top

diff a.txt b.txt
来源：http://qij.gaohongyu789.top

[R55] 压缩与解压
来源：http://xia.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wjb.gotoacloud.top

[R56] 远程拷贝
来源：http://vka.yangfankeji.com

scp file user@host:/path/
来源：http://huy.tian-w.cn

[R57] 远程执行命令
来源：http://xkx.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://jio.sxryk.cn

[R58] 下载文件
来源：http://asx.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ssb.9152youxi.cn

[R59] 发 POST JSON
来源：http://keh.gogol.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vpd.bjfxy.top

[R60] 只看 HTTP 状态码
来源：http://vut.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ljf.aibaodan.cn

[R61] 磁盘占用
来源：http://pjk.gotoacloud.top

df -h;  du -sh *
来源：http://ics.quarkkingdee.top

[R62] 找最占空间的文件
来源：http://zbs.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://nyo.ivvv.top

[R63] 内存与进程
来源：http://mha.c1oappe.top

free -h;  ps aux | grep nginx
来源：http://dig.nwbrower.top

[R64] 结束进程
来源：http://xik.0kj1m.cn

kill -9 $(pgrep -f app.py)
来源：http://sip.shuidangran.top

[R65] 查看端口占用
来源：http://ejo.redwolf501.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hfn.yonumen.top

[R66] 定时任务
来源：http://zcs.xingfuxueyuan.xyz

crontab -e;  crontab -l
来源：http://udj.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://kgw.yuxming.cn

openssl rand -hex 16
来源：http://opq.snrcjt.cn

[R68] 计算文件校验值
来源：http://hpu.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://qek.hongshengwenyu.top

[R69] 生成随机密码
来源：http://amx.zhiwuduotai.top

head -c 16 /dev/urandom | base64
来源：http://psq.sweek.top

[R70] 时间戳与互转
来源：http://tpx.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://clj.mhx1999.top

[R71] 日期格式化
来源：http://mfu.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ooh.hysaishi.cn

[R72] 等待端口就绪
来源：http://ota.hongshengwenyu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nkc.cucudq.cn

[R73] 分割大日志
来源：http://uek.yongpay.top

split -l 1000 big.log part_
来源：http://ueg.daxiang520.top

[R74] 批量重命名
来源：http://bdm.fktsv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uiw.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://rbw.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://hjj.hammf.cn

[R76] 使用临时文件
来源：http://dza.pycfn.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://say.9152youxi.cn

[R77] 读取用户输入
来源：http://uus.yuanzhike.top

read -rp "请输入: " ans
来源：http://fsf.zhengqikj.top

[R78] 交互式菜单
来源：http://cun.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xaq.hcnkem.com

[R79] 解析命令行选项
来源：http://acv.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://esl.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://zmr.yueranfly.top

time ./run.sh
来源：http://nbg.yangfankeji.com

================================================================================
来源：http://dyb.pycfn.com

S. C / C++ 专题
来源：http://nox.daxiang520.top

================================================================================
来源：http://frk.daxiang520.top

[S01] C：Hello World
来源：http://xao.hesvh.cn

#include <stdio.h>
来源：http://bvh.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vof.fzhhl.top

[S02] C：变量与格式化输出
来源：http://aph.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://uwr.daria6918.cn

[S03] C：读入整数
来源：http://zip.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://jqi.52xcode.cn

[S04] C：字符串复制
来源：http://sgx.snrcjt.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bxa.gzhubu.top

[S05] C：字符串长度
来源：http://pfe.shanyushiyangkeji.top

strlen(s)
来源：http://zhu.yonumen.top

[S06] C：字符串比较
来源：http://zty.gogol.net.cn

strcmp(a, b) == 0
来源：http://psa.fengsongda.top

[S07] C：数组遍历求和
来源：http://pgd.nanxinkj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eeu.jinqigufen.top

[S08] C：动态内存分配与释放
来源：http://lbl.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ibk.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://pqo.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iyf.zhongyouzk.top

[S10] C：指针与解引用
来源：http://zsh.hnxiangtu.top

int *p = &a;  *p = 5;
来源：http://jip.bbcook.cn

[S11] C：逐行读文件
来源：http://jhj.aizwys.cn

FILE *f = fopen("a.txt", "r");
来源：http://xvd.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://xrs.hcnkem.com

fclose(f);
来源：http://kvc.ydjk.org.cn

[S12] C：写文件
来源：http://uem.jyoumei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zgs.wangdashe.top

[S13] C：宏定义
来源：http://ddz.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ctr.yj202588.top

[S14] C：枚举
来源：http://sng.zhoulong.xyz

enum Color { RED, GREEN, BLUE };
来源：http://ofx.fanxiaobao.xyz

[S15] C：类型转换
来源：http://slr.nanxuanxn.top

(double) a / b
来源：http://xni.zhengqikj.top

[S16] C：位操作置位
来源：http://dzt.nanxuanxn.top

x |= (1 << 3);
来源：http://xkr.chenjidiqi.icu

[S17] C：安全拼接字符串
来源：http://nzo.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mat.nwbrower.top

[S18] C：命令行参数
来源：http://dge.bbcook.cn

int main(int argc, char **argv)
来源：http://rmy.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://ijz.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bwc.tarul.cn

[S20] C：二分查找
来源：http://dya.jqgfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ckh.hysaishi.cn

[S21] C：字符类别判断
来源：http://dbi.jyoumei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rin.vehdjk.com

[S22] C：字符串转数字
来源：http://hvi.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://rdt.sweek.top

[S23] C：随机数
来源：http://mqf.sxryk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kjj.zhiwuduotai.top

[S24] C：获取本地时间
来源：http://rsh.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rab.fengsongda.top

[S25] C：内存拷贝
来源：http://ity.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://wqp.gogol.net.cn

[S26] C：内存清零
来源：http://pae.yj20258.top

memset(a, 0, sizeof a);
来源：http://pwm.hnxiangtu.top

[S27] C：定义常量
来源：http://aak.daxiang520.top

const double PI = 3.14159;
来源：http://uza.xinyue.icu

[S28] C：静态变量
来源：http://aqd.dianchejie.cn

static int counter = 0;
来源：http://noy.yj20258.top

[S29] C：变参函数
来源：http://jjo.cdnleiting.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pmz.0kj1m.cn

[S30] C：头文件保护
来源：http://fnb.nanxuanxn.top

#ifndef X_H
来源：http://nle.pycfn.com

#define X_H
来源：http://vzr.316326.xyz

#endif
来源：http://huy.mhx1999.top

[S31] C++：Hello World
来源：http://fva.redwolf501.top

#include <iostream>
来源：http://zyi.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://xgh.wangdashe.top

[S32] C++：字符串
来源：http://ipi.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://pgb.nanxinkj.top

[S33] C++：vector 增删
来源：http://fvu.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qsw.smart0.xyz

[S34] C++：遍历 vector
来源：http://opx.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://noo.0kj1m.cn

[S35] C++：map
来源：http://vsm.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nse.birdmap.top

[S36] C++：unordered_map
来源：http://mro.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dru.zhiwuduotai.top

[S37] C++：set
来源：http://cnr.zdbjq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vhq.zdqjudy.top

[S38] C++：排序
来源：http://icw.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://alj.svipenyu.cn

[S39] C++：自定义比较器排序
来源：http://pgt.yueranfly.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mlk.52xcode.cn

[S40] C++：查找元素
来源：http://nyn.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mxh.yuxming.cn

[S41] C++：类与构造函数
来源：http://rnu.kuanghao11.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qgy.hcnkem.com

[S42] C++：继承与虚函数
来源：http://cgu.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://igk.cdnleiting.top

[S43] C++：智能指针
来源：http://gfc.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://ulz.jiagoushi.top

[S44] C++：引用传参
来源：http://vph.sysykeji.top

void inc(int &x) { ++x; }
来源：http://znk.shanyushiyangtech.top

[S45] C++：lambda
来源：http://uoc.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://srv.jqgfzy.top

[S46] C++：函数模板
来源：http://vuv.shanyushiyangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fpe.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://fjw.hesvh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://beo.birdmap.top

[S48] C++：逐行读文件
来源：http://fue.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gfr.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://cag.wangdashe.top

[S49] C++：写文件
来源：http://ltu.nanxinkj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pyn.0kj1m.cn

[S50] C++：格式化数字
来源：http://klt.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lpf.sweek.top

[S51] C++：显式类型转换
来源：http://fvj.tian-w.cn

static_cast<double>(a) / b
来源：http://sxg.ydzc1.top

[S52] C++：const 与 noexcept
来源：http://ajo.yonumen.top

int size() const noexcept { return n_; }
来源：http://sav.sjlbkw.cn

[S53] C++：移动语义
来源：http://jqi.gotoacloud.top

std::vector<int> w = std::move(v);
来源：http://fak.52xcode.cn

[S54] C++：异常处理
来源：http://fkr.uphjek.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ged.yfazqb.com

[S55] C++：结构化绑定
来源：http://euh.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gyf.jiagoushi.top

[S56] C++：optional
来源：http://tbk.guannengcc.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zaz.haohaochexian.top

[S57] C++：编译期常量
来源：http://zhz.bjfxy.top

constexpr int N = 10;
来源：http://tck.jyoumei.cn

[S58] C++：命名空间
来源：http://vws.daxiang520.top

namespace ns { int f() { return 1; } }
来源：http://vme.guannengcc.top

[S59] C++：静态断言
来源：http://pbx.cqqwz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qjd.zhijiandao.cn

[S60] C++：遍历并删除元素
来源：http://der.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gfh.shzxlz.cn

================================================================================
来源：http://bsv.xuanzx.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://far.jinghuilouyu.cn

================================================================================
来源：http://ris.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://vlt.fengsongda.top

println("Hello")
来源：http://cas.yangfankeji.com

[T02] Kotlin：变量
来源：http://oux.jinghuilouyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hxa.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://oid.chenzaomai.com

"值: $b"
来源：http://edh.wangdashe.top

[T04] Kotlin：空安全
来源：http://jan.chenzaomai.com

val n: String? = null;  n?.length
来源：http://xqh.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://pit.ppjwa.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lrx.nwbrower.top

[T06] Kotlin：集合映射
来源：http://era.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zkq.shanyushiyangkeji.top

[T07] Kotlin：集合过滤
来源：http://hku.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zzb.gotoacloud.top

[T08] Kotlin：数据类
来源：http://nix.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://tli.zhixingplan.top

[T09] Kotlin：扩展函数
来源：http://gzo.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://lxl.bbcook.cn

[T10] Kotlin：默认参数
来源：http://ajs.ehwqpu.com

fun greet(name: String = "World") = "Hi $name"
来源：http://opc.ehwqpu.com


<!-- 参考信息 -->