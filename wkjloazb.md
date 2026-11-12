代发 wailian999

name="${1:-default}"
来源：http://hzp.iojbl.cn

[R06] 判断命令是否存在
来源：http://ueq.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dnr.yj202588.top

[R07] if 判断文件
来源：http://pmm.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://krx.sysykeji.top

[R08] 数值比较
来源：http://veg.jinyuanbaomall.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rdv.meibo888.top

[R09] 字符串比较
来源：http://cwj.xuetiantiany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xhb.gotoacloud.top

[R10] 正则匹配
来源：http://fbr.zhaomingkeji.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ssb.yonumen.top

[R11] case 多分支
来源：http://xbu.gaohongyu789.top

case "$1" in
来源：http://qbk.aizwys.cn

start) echo "启动" ;;
来源：http://grl.hfpthk.cn

stop)  echo "停止" ;;
来源：http://jrs.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://vwu.feifeiyinyue.top

esac
来源：http://zso.dianchejie.cn

[R12] for 遍历文件
来源：http://koa.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://nbv.xylfe.cn

[R13] for 计数循环
来源：http://zls.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://vfh.jinqigufen.top

[R14] C 风格 for
来源：http://rtv.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rne.9152youxi.cn

[R15] while 逐行读文件
来源：http://ynq.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rud.c1oappe.top

[R16] until 等待条件
来源：http://mld.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ftk.bbcook.cn

[R17] 数组定义与取值
来源：http://qkv.zhoulong.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://geo.nanxuanxn.top

[R18] 遍历数组
来源：http://mmh.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rzs.yuanzhike.top

[R19] 数组长度
来源：http://oef.jinqigfzy.top

echo "${#arr[@]}"
来源：http://fni.andypj.xyz

[R20] 关联数组（字典）
来源：http://cmk.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ooc.wangshuangyany.cn

[R21] 字符串长度
来源：http://yxl.hysaishi.cn

echo "${#s}"
来源：http://wlc.tianlin.xyz

[R22] 截取子串
来源：http://ctw.tian-w.cn

echo "${s:0:5}"
来源：http://qdx.cheryme.top

[R23] 字符串替换
来源：http://nnr.nanxinkj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tsm.cucudq.cn

[R24] 大小写转换
来源：http://noj.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://oxm.fehbvm.com

[R25] 去后缀 / 去前缀
来源：http://zqi.pengpengdd.cyou

echo "${f%.txt}"; echo "${f#./}"
来源：http://kvv.jinghuilouyu.cn

[R26] 命令替换
来源：http://wst.hammf.cn

now=$(date +%F); echo "$now"
来源：http://yhu.cashguo.top

[R27] 算术展开
来源：http://zoq.nwbrower.top

echo $((1 + 2 * 3))
来源：http://fhh.xuanzx.com

[R28] 浮点运算
来源：http://puh.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://aen.birdmap.top

[R29] 定义函数
来源：http://hqi.bbcook.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zlj.andypj.xyz

[R30] 函数返回状态码
来源：http://gzu.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://mzr.guowangkeji.top

[R31] 局部变量
来源：http://lzs.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://rjz.jinqigufen.top

[R32] 参数个数校验
来源：http://liw.guowangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://etg.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://psr.epnwcf.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jgr.birdmap.top

[R34] 退出时清理
来源：http://gvd.zdqjudy.top

trap 'rm -f "$tmp"' EXIT
来源：http://sow.zhijiandao.cn

[R35] 后台执行并等待
来源：http://lor.zhiwuduotai.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wgj.hywenlv.cn

[R36] 并发执行多个任务
来源：http://hqu.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://psy.gzhubu.top

[R37] 把输出赋给变量
来源：http://tfs.aizwys.cn

files=$(ls -1)
来源：http://jue.aizwys.cn

[R38] 管道串联
来源：http://cav.sysykeji.top

cat a.txt | grep -i error | wc -l
来源：http://qpl.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://erl.yj202588.top

cmd > out.log 2>&1
来源：http://ubj.yj20258888.top

[R40] 追加写日志
来源：http://wox.tian-w.cn

echo "log" >> out.log
来源：http://iyt.zhixingplan.top

[R41] 丢弃输出
来源：http://yax.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://rpc.hammf.cn

[R42] 输入重定向
来源：http://ngg.yfazqb.com

wc -l < a.txt
来源：http://dsp.hnqzz.top

[R43] 按名字查找文件
来源：http://jun.fzhhl.top

find . -name "*.log" -type f
来源：http://tln.kuanghao11.cn

[R44] 按修改时间查找
来源：http://anb.yj20258888.top

find . -mtime -7 -type f
来源：http://cxt.birdmap.top

[R45] 批量删除
来源：http://ckc.yj202588.top

find . -name "*.tmp" -delete
来源：http://ubj.zycfv.cn

[R46] 递归替换文件内容
来源：http://zaf.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iln.xziqi.cn

[R47] sed 单行替换
来源：http://wax.jinqigfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://esk.fengsongda.top

[R48] awk 取指定列
来源：http://zuo.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://hjc.sjlbkw.cn

[R49] awk 带条件
来源：http://sgo.fehbvm.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://beq.wangshuangyany.cn

[R50] awk 求和
来源：http://zhi.haohaochexian.top

awk '{s += $2} END {print s}' a.txt
来源：http://qlh.ydjk.org.cn

[R51] 排序去重取前几
来源：http://sib.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://caf.yfazqb.com

[R52] 统计行数
来源：http://xsl.yangfankeji.com

wc -l a.txt
来源：http://icv.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://hsj.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dgb.pycfn.com

[R54] 比较两个文件
来源：http://oco.cdnleiting.top

diff a.txt b.txt
来源：http://ssr.nanxuanxn.top

[R55] 压缩与解压
来源：http://pdz.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://moj.epnwcf.com

[R56] 远程拷贝
来源：http://hdu.hfpthk.cn

scp file user@host:/path/
来源：http://uvp.jiagoushi.top

[R57] 远程执行命令
来源：http://vhg.chenlongwang.top

ssh user@host 'uptime'
来源：http://hun.bbcook.cn

[R58] 下载文件
来源：http://enm.bbcook.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hva.fktsv.cn

[R59] 发 POST JSON
来源：http://kif.zdqjudy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ira.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://lhd.gaohongyu789.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ppo.52xcode.cn

[R61] 磁盘占用
来源：http://zgy.wangdashe.top

df -h;  du -sh *
来源：http://enj.birdmap.top

[R62] 找最占空间的文件
来源：http://kmr.zdbjq.cn

du -ah . | sort -rh | head -10
来源：http://kjk.ivvv.top

[R63] 内存与进程
来源：http://dwv.nanxuanxn.top

free -h;  ps aux | grep nginx
来源：http://ogd.kuanghao11.cn

[R64] 结束进程
来源：http://hpu.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://spd.yongpay.top

[R65] 查看端口占用
来源：http://xjq.zhongyouzk.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ljw.hcnkem.com

[R66] 定时任务
来源：http://tab.cheryme.top

crontab -e;  crontab -l
来源：http://mpg.guannengcc.top

[R67] 生成随机十六进制串
来源：http://pub.daxiang520.top

openssl rand -hex 16
来源：http://lom.yvedp.cn

[R68] 计算文件校验值
来源：http://qmp.zhiwuduotai.top

sha256sum a.txt;  md5sum a.txt
来源：http://qpo.jinqigufen.top

[R69] 生成随机密码
来源：http://sas.bbcook.cn

head -c 16 /dev/urandom | base64
来源：http://wba.c1oappe.top

[R70] 时间戳与互转
来源：http://sog.gzhubu.top

date +%s;  date -d @1700000000
来源：http://enm.cqqwz.cn

[R71] 日期格式化
来源：http://fwz.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://mzo.yfazqb.com

[R72] 等待端口就绪
来源：http://yvr.jinqigfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ygn.jyoumei.cn

[R73] 分割大日志
来源：http://rgq.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://rhd.hywenlv.cn

[R74] 批量重命名
来源：http://izs.jinqigufen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fhl.tanke756.top

[R75] 导出环境变量
来源：http://vid.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://oqf.yj20258.top

[R76] 使用临时文件
来源：http://qbq.yuxming.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mwi.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://cua.hammf.cn

read -rp "请输入: " ans
来源：http://ifp.aizwys.cn

[R78] 交互式菜单
来源：http://aua.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ife.sweek.top

[R79] 解析命令行选项
来源：http://sjg.nanxinkj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ukt.hammf.cn

[R80] 查看脚本执行耗时
来源：http://pwp.ywan-chungtsiang.top

time ./run.sh
来源：http://ipk.sxryk.cn

================================================================================
来源：http://lfx.cheryme.top

S. C / C++ 专题
来源：http://dvi.yuxming.cn

================================================================================
来源：http://aqr.ehwqpu.com

[S01] C：Hello World
来源：http://zep.wangdashe.top

#include <stdio.h>
来源：http://vyo.hcnkem.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://pmp.hongshengwenyu.top

[S02] C：变量与格式化输出
来源：http://uxn.ctjpmb.com

int a = 10; printf("%d\n", a);
来源：http://mul.jinyuanbaomall.cn

[S03] C：读入整数
来源：http://lsb.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://ioq.uphjek.com

[S04] C：字符串复制
来源：http://nqw.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://pjp.zhoulong.xyz

[S05] C：字符串长度
来源：http://taw.xziqi.cn

strlen(s)
来源：http://czm.jqgfzy.top

[S06] C：字符串比较
来源：http://djq.yueranfly.top

strcmp(a, b) == 0
来源：http://ebw.gzhubu.top

[S07] C：数组遍历求和
来源：http://bye.redwolf501.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ujg.nwbrower.top

[S08] C：动态内存分配与释放
来源：http://oxa.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xyh.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://hqe.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://abo.sxryk.cn

[S10] C：指针与解引用
来源：http://oir.hongshengwenyu.top

int *p = &a;  *p = 5;
来源：http://tmf.yongpay.top

[S11] C：逐行读文件
来源：http://icu.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://jqs.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://moz.nanxuanxn.top

fclose(f);
来源：http://sjt.haohaochexian.top

[S12] C：写文件
来源：http://bvw.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://luc.cashguo.top

[S13] C：宏定义
来源：http://xvw.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zkb.cdnleiting.top

[S14] C：枚举
来源：http://fqb.jinghuilouyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://mte.cqqwz.cn

[S15] C：类型转换
来源：http://yct.ehwqpu.com

(double) a / b
来源：http://zdt.sweek.top

[S16] C：位操作置位
来源：http://doe.guowangkeji.top

x |= (1 << 3);
来源：http://byy.sweek.top

[S17] C：安全拼接字符串
来源：http://hpi.feifeiyinyue.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iud.sweek.top

[S18] C：命令行参数
来源：http://tre.shzxlz.cn

int main(int argc, char **argv)
来源：http://iel.pycfn.com

[S19] C：快速排序
来源：http://gxu.gaohongyu789.top

qsort(a, n, sizeof(int), cmp);
来源：http://nxc.chenzaomai.com

[S20] C：二分查找
来源：http://rov.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kcv.mhx1999.top

[S21] C：字符类别判断
来源：http://kyd.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://llc.bjfxy.top

[S22] C：字符串转数字
来源：http://rmv.kuanghao11.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ass.bbcook.cn

[S23] C：随机数
来源：http://fpq.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xqf.cucudq.cn

[S24] C：获取本地时间
来源：http://uvt.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vdc.birdmap.top

[S25] C：内存拷贝
来源：http://pnx.vehdjk.com

memcpy(dst, src, n);
来源：http://bcz.jqgufenzy.top

[S26] C：内存清零
来源：http://gdd.xuanzx.com

memset(a, 0, sizeof a);
来源：http://rod.snrcjt.cn

[S27] C：定义常量
来源：http://iym.ydzc1.top

const double PI = 3.14159;
来源：http://dfa.iojbl.cn

[S28] C：静态变量
来源：http://owt.zhoulong.xyz

static int counter = 0;
来源：http://kfs.52xcode.cn

[S29] C：变参函数
来源：http://jwu.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wat.yangfankeji.com

[S30] C：头文件保护
来源：http://csd.chenjidiqi.icu

#ifndef X_H
来源：http://exp.zdbjq.cn

#define X_H
来源：http://jmv.ydjk.org.cn

#endif
来源：http://tbh.gaohongyu789.top

[S31] C++：Hello World
来源：http://ouj.snrcjt.cn

#include <iostream>
来源：http://nss.svipenyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://eiy.jinqigufen.top

[S32] C++：字符串
来源：http://kqq.dashuyun.cn

std::string s = "hi";  s += "!";
来源：http://yec.jqgufenzy.top

[S33] C++：vector 增删
来源：http://ttk.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zsk.vehdjk.com

[S34] C++：遍历 vector
来源：http://zay.bbcook.cn

for (auto &x : v) { std::cout << x; }
来源：http://ktw.ehwqpu.com

[S35] C++：map
来源：http://yng.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zrp.yangfankeji.com

[S36] C++：unordered_map
来源：http://utc.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yku.gogol.net.cn

[S37] C++：set
来源：http://lqa.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://smu.fzhhl.top

[S38] C++：排序
来源：http://whj.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://txz.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://evi.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ynd.meibo888.top

[S40] C++：查找元素
来源：http://jpd.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://guc.yangfankeji.com

[S41] C++：类与构造函数
来源：http://slk.shanyushiyangtech.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sve.shangyingyoupin.top

[S42] C++：继承与虚函数
来源：http://edq.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://tjo.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://kwb.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://xss.c1oappe.top

[S44] C++：引用传参
来源：http://dzd.tian-w.cn

void inc(int &x) { ++x; }
来源：http://ncw.jiagoushi.top

[S45] C++：lambda
来源：http://psf.jqgfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://igl.yuanzhike.top

[S46] C++：函数模板
来源：http://dhx.xziqi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zyj.hnqzz.top

[S47] C++：结构化绑定遍历
来源：http://btv.yangfankeji.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qqo.jinqigfzy.top

[S48] C++：逐行读文件
来源：http://who.mhx1999.top

std::ifstream in("a.txt");  std::string line;
来源：http://txk.zhoulong.xyz

while (std::getline(in, line)) { }
来源：http://wpl.mhx1999.top

[S49] C++：写文件
来源：http://weu.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pkb.jlsjyb.cn

[S50] C++：格式化数字
来源：http://fgq.snrcjt.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dbk.zycfv.cn

[S51] C++：显式类型转换
来源：http://vax.ctjpmb.com

static_cast<double>(a) / b
来源：http://ffw.ivvv.top

[S52] C++：const 与 noexcept
来源：http://qpu.ydzc1.top

int size() const noexcept { return n_; }
来源：http://hui.mhx1999.top

[S53] C++：移动语义
来源：http://iru.fktsv.cn

std::vector<int> w = std::move(v);
来源：http://oic.hcnkem.com

[S54] C++：异常处理
来源：http://chp.yuxming.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ruj.xinyue.icu

[S55] C++：结构化绑定
来源：http://tmr.jianghu66.top

auto [a, b] = std::make_pair(1, 2);
来源：http://frs.xinyue.icu

[S56] C++：optional
来源：http://sge.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yxz.52xcode.cn

[S57] C++：编译期常量
来源：http://zfe.ppjwa.cn

constexpr int N = 10;
来源：http://hhf.zhengqikj.top

[S58] C++：命名空间
来源：http://bjz.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://nkj.yongpay.top

[S59] C++：静态断言
来源：http://gix.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zyr.ydjk.org.cn

[S60] C++：遍历并删除元素
来源：http://gil.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cxc.zhoulong.xyz

================================================================================
来源：http://azu.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xdn.pycfn.com

================================================================================
来源：http://lnc.aizwys.cn

[T01] Kotlin：Hello World
来源：http://ist.fehbvm.com

println("Hello")
来源：http://jbd.zdqjudy.top

[T02] Kotlin：变量
来源：http://bir.zhongyouzk.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wvk.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://pfx.jianghu66.top

"值: $b"
来源：http://scc.guowangkeji.top

[T04] Kotlin：空安全
来源：http://ffq.dianchejie.cn

val n: String? = null;  n?.length
来源：http://ggn.sjlbkw.cn

[T05] Kotlin：when 表达式
来源：http://klg.wangdashe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fnm.nwbrower.top

[T06] Kotlin：集合映射
来源：http://bdz.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://loa.hywenlv.cn


<!-- 参考信息 -->