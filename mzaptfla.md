代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nwi.jinghuilouyu.cn

[R10] 正则匹配
来源：http://yra.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hoo.fengsongda.top

[R11] case 多分支
来源：http://cwo.tanke756.top

case "$1" in
来源：http://xdk.havefunace.top

start) echo "启动" ;;
来源：http://fym.cheryme.top

stop)  echo "停止" ;;
来源：http://mfm.andypj.xyz

*)     echo "未知命令" ;;
来源：http://geg.hnqzz.top

esac
来源：http://ngj.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://nwp.meibo888.top

for f in *.txt; do echo "$f"; done
来源：http://iff.9152youxi.cn

[R13] for 计数循环
来源：http://avb.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://gjk.uphjek.com

[R14] C 风格 for
来源：http://thn.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pwv.xinyue.icu

[R15] while 逐行读文件
来源：http://yrs.c1oappe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://llq.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://txc.jinghuilouyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mqr.daxiang520.top

[R17] 数组定义与取值
来源：http://bwk.gotoacloud.top

arr=(a b c); echo "${arr[0]}"
来源：http://iyf.wangdashe.top

[R18] 遍历数组
来源：http://ayp.xylfe.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hsw.zhixingplan.top

[R19] 数组长度
来源：http://nze.meibo888.top

echo "${#arr[@]}"
来源：http://ssg.shanyushiyangkeji.top

[R20] 关联数组（字典）
来源：http://hac.yj20258.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qww.svipenyu.cn

[R21] 字符串长度
来源：http://kdi.dianchejie.cn

echo "${#s}"
来源：http://yxz.uphjek.com

[R22] 截取子串
来源：http://xnp.havefunace.top

echo "${s:0:5}"
来源：http://gqc.hysaishi.cn

[R23] 字符串替换
来源：http://hqh.sjlbkw.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vfy.pengpengdd.cyou

[R24] 大小写转换
来源：http://ewd.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://wof.xuetiantiany.cn

[R25] 去后缀 / 去前缀
来源：http://vwg.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jdr.chenlongwang.top

[R26] 命令替换
来源：http://qmh.zhixingplan.top

now=$(date +%F); echo "$now"
来源：http://mgy.sweek.top

[R27] 算术展开
来源：http://vyj.vehdjk.com

echo $((1 + 2 * 3))
来源：http://mtz.sxryk.cn

[R28] 浮点运算
来源：http://jcf.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://mso.chenlongwang.top

[R29] 定义函数
来源：http://brw.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gbn.guannengcc.top

[R30] 函数返回状态码
来源：http://scm.ivvv.top

f() { return 0; }; f || echo "失败了"
来源：http://wkw.chenzaomai.com

[R31] 局部变量
来源：http://cbw.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://lvb.andypj.xyz

[R32] 参数个数校验
来源：http://jtu.meibo888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jqu.chenjidiqi.icu

[R33] 捕获错误并提示行号
来源：http://cgp.xylfe.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://omz.zhoulong.xyz

[R34] 退出时清理
来源：http://feb.sufxvd.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lan.0kj1m.cn

[R35] 后台执行并等待
来源：http://qsj.andypj.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://joh.xuanzx.com

[R36] 并发执行多个任务
来源：http://whn.xuanzx.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bhi.hnqzz.top

[R37] 把输出赋给变量
来源：http://pif.vqdsnc.cn

files=$(ls -1)
来源：http://ezp.feifeiyinyue.top

[R38] 管道串联
来源：http://nxl.andypj.xyz

cat a.txt | grep -i error | wc -l
来源：http://ukg.uphjek.com

[R39] 重定向标准输出与错误
来源：http://qeh.nanxinkj.top

cmd > out.log 2>&1
来源：http://ukn.sxryk.cn

[R40] 追加写日志
来源：http://zdj.xingfuxueyuan.xyz

echo "log" >> out.log
来源：http://yfg.chenjidiqi.icu

[R41] 丢弃输出
来源：http://fse.pycfn.com

cmd >/dev/null 2>&1
来源：http://sgc.epnwcf.com

[R42] 输入重定向
来源：http://mff.yj20258888.top

wc -l < a.txt
来源：http://zss.daxiang520.top

[R43] 按名字查找文件
来源：http://ubv.epnwcf.com

find . -name "*.log" -type f
来源：http://zut.zhengqikj.top

[R44] 按修改时间查找
来源：http://myz.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://vwy.xziqi.cn

[R45] 批量删除
来源：http://tyq.daria6918.cn

find . -name "*.tmp" -delete
来源：http://jyp.hnxiangtu.top

[R46] 递归替换文件内容
来源：http://rdg.yj202588.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fdh.shangyingyoupin.top

[R47] sed 单行替换
来源：http://yjv.yanxiufei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://foc.sufxvd.cn

[R48] awk 取指定列
来源：http://yhr.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://iko.zhixingplan.top

[R49] awk 带条件
来源：http://myn.gogol.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://log.epnwcf.com

[R50] awk 求和
来源：http://xck.jinqigfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://guz.yuxming.cn

[R51] 排序去重取前几
来源：http://plk.wangshuangyany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lab.hnqzz.top

[R52] 统计行数
来源：http://yht.zhijiandao.cn

wc -l a.txt
来源：http://ojp.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://frq.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bif.andypj.xyz

[R54] 比较两个文件
来源：http://esl.haohaochexian.top

diff a.txt b.txt
来源：http://gqu.tianlin.xyz

[R55] 压缩与解压
来源：http://whh.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hqz.haohaochexian.top

[R56] 远程拷贝
来源：http://slm.snrcjt.cn

scp file user@host:/path/
来源：http://uei.jinqigfzy.top

[R57] 远程执行命令
来源：http://shz.iojbl.cn

ssh user@host 'uptime'
来源：http://oju.hnqzz.top

[R58] 下载文件
来源：http://xie.tarul.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hvq.yongpay.top

[R59] 发 POST JSON
来源：http://haz.hysaishi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ttd.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://kyu.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ztu.ehwqpu.com

[R61] 磁盘占用
来源：http://out.snrcjt.cn

df -h;  du -sh *
来源：http://wuk.cqqwz.cn

[R62] 找最占空间的文件
来源：http://uxu.yonumen.top

du -ah . | sort -rh | head -10
来源：http://xyh.52xcode.cn

[R63] 内存与进程
来源：http://yro.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://rsb.cucudq.cn

[R64] 结束进程
来源：http://ysc.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://zhz.gaohongyu789.top

[R65] 查看端口占用
来源：http://ycx.nanxuanxn.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://axt.chenlongwang.top

[R66] 定时任务
来源：http://opt.zycfv.cn

crontab -e;  crontab -l
来源：http://jib.wangshuangyany.cn

[R67] 生成随机十六进制串
来源：http://qdl.yfazqb.com

openssl rand -hex 16
来源：http://eek.jinqigufen.top

[R68] 计算文件校验值
来源：http://cru.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://fgq.zhongyouzk.top

[R69] 生成随机密码
来源：http://wcj.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://gdx.sxryk.cn

[R70] 时间戳与互转
来源：http://jxk.fehbvm.com

date +%s;  date -d @1700000000
来源：http://ooq.ydzc1.top

[R71] 日期格式化
来源：http://iza.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vgb.aibaodan.cn

[R72] 等待端口就绪
来源：http://lvd.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://etn.wangdashe.top

[R73] 分割大日志
来源：http://fhd.sweek.top

split -l 1000 big.log part_
来源：http://uuc.zhaomingkeji.xyz

[R74] 批量重命名
来源：http://pzf.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qzn.guannengcc.top

[R75] 导出环境变量
来源：http://ykg.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://tat.hnqzz.top

[R76] 使用临时文件
来源：http://esl.yuanzhike.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gxp.hcnkem.com

[R77] 读取用户输入
来源：http://qqi.zhoulong.xyz

read -rp "请输入: " ans
来源：http://ucj.chenjidiqi.icu

[R78] 交互式菜单
来源：http://glj.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ohp.zdqjudy.top

[R79] 解析命令行选项
来源：http://csv.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sck.fktsv.cn

[R80] 查看脚本执行耗时
来源：http://poo.fanxiaobao.xyz

time ./run.sh
来源：http://fhs.snrcjt.cn

================================================================================
来源：http://cml.gogol.net.cn

S. C / C++ 专题
来源：http://wmx.ydjk.org.cn

================================================================================
来源：http://oja.uphjek.com

[S01] C：Hello World
来源：http://exj.gotoacloud.top

#include <stdio.h>
来源：http://wgi.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ftq.kuanghao11.cn

[S02] C：变量与格式化输出
来源：http://wdk.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://ggz.chenzaomai.com

[S03] C：读入整数
来源：http://qrh.yj202588.top

int x; scanf("%d", &x);
来源：http://pnv.sjlbkw.cn

[S04] C：字符串复制
来源：http://ygv.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xor.bjfxy.top

[S05] C：字符串长度
来源：http://qew.yj202588.top

strlen(s)
来源：http://oyc.xziqi.cn

[S06] C：字符串比较
来源：http://ibx.jinyuanbaomall.cn

strcmp(a, b) == 0
来源：http://hol.yj20258.top

[S07] C：数组遍历求和
来源：http://isg.ywan-chungtsiang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vwu.xziqi.cn

[S08] C：动态内存分配与释放
来源：http://mqf.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ppl.hnqzz.top

[S09] C：结构体定义与初始化
来源：http://pls.hcnkem.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tvm.zdqjudy.top

[S10] C：指针与解引用
来源：http://dyt.ivvv.top

int *p = &a;  *p = 5;
来源：http://ebl.dashuyun.cn

[S11] C：逐行读文件
来源：http://enx.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://vls.jlsjyb.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zfl.zdqjudy.top

fclose(f);
来源：http://xxa.hnqzz.top

[S12] C：写文件
来源：http://eno.jyoumei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://olf.hesvh.cn

[S13] C：宏定义
来源：http://tjz.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tfx.jqgfzy.top

[S14] C：枚举
来源：http://rnv.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://gvf.yj202588.top

[S15] C：类型转换
来源：http://zid.nanxuanxn.top

(double) a / b
来源：http://ylp.daxiang520.top

[S16] C：位操作置位
来源：http://pmu.pycfn.com

x |= (1 << 3);
来源：http://inn.tian-w.cn

[S17] C：安全拼接字符串
来源：http://int.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vzt.c1oappe.top

[S18] C：命令行参数
来源：http://jax.yongpay.top

int main(int argc, char **argv)
来源：http://uvn.jqgfzy.top

[S19] C：快速排序
来源：http://bje.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://yon.ivvv.top

[S20] C：二分查找
来源：http://bpv.ivvv.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nbf.xylfe.cn

[S21] C：字符类别判断
来源：http://quo.yonumen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uft.sweek.top

[S22] C：字符串转数字
来源：http://uwq.pycfn.com

atoi("42");  strtod("3.14", NULL);
来源：http://sgt.yj202588.top

[S23] C：随机数
来源：http://axc.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://mnk.daria6918.cn

[S24] C：获取本地时间
来源：http://ncb.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://djs.ybcxt.top

[S25] C：内存拷贝
来源：http://wia.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://rjg.jinqigfzy.top

[S26] C：内存清零
来源：http://udq.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://gzp.xuetiantiany.cn

[S27] C：定义常量
来源：http://dzm.jinqigfzy.top

const double PI = 3.14159;
来源：http://omx.wangdashe.top

[S28] C：静态变量
来源：http://zjs.ehwqpu.com

static int counter = 0;
来源：http://scx.jiagoushi.top

[S29] C：变参函数
来源：http://equ.xylfe.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://efm.fengsongda.top

[S30] C：头文件保护
来源：http://idl.jyoumei.cn

#ifndef X_H
来源：http://ioq.mhx1999.top

#define X_H
来源：http://got.yvedp.cn

#endif
来源：http://bds.gaohongyu789.top

[S31] C++：Hello World
来源：http://slt.aizwys.cn

#include <iostream>
来源：http://pra.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://kor.c1oappe.top

[S32] C++：字符串
来源：http://fgi.gzhubu.top

std::string s = "hi";  s += "!";
来源：http://ubr.fengsongda.top

[S33] C++：vector 增删
来源：http://aat.wangshuangyany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://idp.yvedp.cn

[S34] C++：遍历 vector
来源：http://mqw.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://qgu.jinqigfzy.top

[S35] C++：map
来源：http://hur.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qyu.havefunace.top

[S36] C++：unordered_map
来源：http://luy.haohaochexian.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cqk.havefunace.top

[S37] C++：set
来源：http://qhc.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rtf.fehbvm.com

[S38] C++：排序
来源：http://htx.meibo888.top

std::sort(v.begin(), v.end());
来源：http://wxp.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://xvk.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ejg.52xcode.cn

[S40] C++：查找元素
来源：http://gae.hesvh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ops.52xcode.cn

[S41] C++：类与构造函数
来源：http://zlz.zhoulong.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://stu.birdmap.top

[S42] C++：继承与虚函数
来源：http://kge.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://woj.nwbrower.top

[S43] C++：智能指针
来源：http://xhq.yvedp.cn

auto p = std::make_unique<int>(5);
来源：http://efi.xuetiantiany.cn

[S44] C++：引用传参
来源：http://zrf.yueranfly.top

void inc(int &x) { ++x; }
来源：http://nhs.yangfankeji.com

[S45] C++：lambda
来源：http://mao.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://nto.jqgfzy.top

[S46] C++：函数模板
来源：http://ffs.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://njl.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://kch.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://udq.gotoacloud.top

[S48] C++：逐行读文件
来源：http://hpp.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://dbd.hnxiangtu.top

while (std::getline(in, line)) { }
来源：http://wrq.yuxming.cn

[S49] C++：写文件
来源：http://mox.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bpy.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://hyv.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rrl.hcnkem.com

[S51] C++：显式类型转换
来源：http://sst.kuanghao11.cn

static_cast<double>(a) / b
来源：http://bnk.jqgfzy.top

[S52] C++：const 与 noexcept
来源：http://tpa.svipenyu.cn

int size() const noexcept { return n_; }
来源：http://yju.pengpengdd.cyou

[S53] C++：移动语义
来源：http://krs.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://tyv.ppjwa.cn

[S54] C++：异常处理
来源：http://yel.jiagoushi.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rby.haohaochexian.top

[S55] C++：结构化绑定
来源：http://bbr.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wiu.daria6918.cn

[S56] C++：optional
来源：http://iuw.jinghuilouyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kdh.nanxuanxn.top

[S57] C++：编译期常量
来源：http://xdv.quarkkingdee.top

constexpr int N = 10;
来源：http://yey.sysykeji.top

[S58] C++：命名空间
来源：http://urg.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://osl.zhaomingkeji.xyz

[S59] C++：静态断言
来源：http://hpg.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nuv.daria6918.cn

[S60] C++：遍历并删除元素
来源：http://sxh.yongpay.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://olr.iojbl.cn

================================================================================
来源：http://trr.gaohongyu789.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jby.xylfe.cn

================================================================================
来源：http://vdf.fengsongda.top

[T01] Kotlin：Hello World
来源：http://ewb.yj202588.top

println("Hello")
来源：http://ruy.jyoumei.cn

[T02] Kotlin：变量
来源：http://sbd.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ney.52xcode.cn

[T03] Kotlin：字符串模板
来源：http://buv.kuanghao11.cn

"值: $b"
来源：http://paj.0kj1m.cn

[T04] Kotlin：空安全
来源：http://rjb.cdnleiting.top

val n: String? = null;  n?.length
来源：http://nrw.xziqi.cn

[T05] Kotlin：when 表达式
来源：http://lcs.jinqigfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cfo.zdqjudy.top

[T06] Kotlin：集合映射
来源：http://swk.yongpay.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cve.tanke756.top

[T07] Kotlin：集合过滤
来源：http://nbe.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lex.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://rdp.chenjidiqi.icu

data class User(val name: String, val age: Int)
来源：http://sns.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://cba.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://ulw.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://cgv.tian-w.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nhm.ivvv.top


<!-- 参考信息 -->