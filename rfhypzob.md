代发 wailian999

readonly PI=3.14
来源：http://rhq.ybcxt.top

[R04] 位置参数
来源：http://glu.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mib.jiagoushi.top

[R05] 参数默认值
来源：http://nil.hysaishi.cn

name="${1:-default}"
来源：http://rzv.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://djn.gotoacloud.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://txd.hongshengwenyu.top

[R07] if 判断文件
来源：http://fyv.redwolf501.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wzw.andypj.xyz

[R08] 数值比较
来源：http://mrg.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://odm.tanke756.top

[R09] 字符串比较
来源：http://jjq.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tkq.316326.xyz

[R10] 正则匹配
来源：http://clg.hammf.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fdn.fehbvm.com

[R11] case 多分支
来源：http://rrp.yvedp.cn

case "$1" in
来源：http://veq.hywenlv.cn

start) echo "启动" ;;
来源：http://vev.nanxuanxn.top

stop)  echo "停止" ;;
来源：http://dnh.meibo888.top

*)     echo "未知命令" ;;
来源：http://orm.vqdsnc.cn

esac
来源：http://qho.aizwys.cn

[R12] for 遍历文件
来源：http://cat.svipenyu.cn

for f in *.txt; do echo "$f"; done
来源：http://myp.sxryk.cn

[R13] for 计数循环
来源：http://ugy.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://vve.tianlin.xyz

[R14] C 风格 for
来源：http://bhe.chenzaomai.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bzi.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://dvu.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://owo.sysykeji.top

[R16] until 等待条件
来源：http://sse.hnqzz.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mlh.ydzc1.top

[R17] 数组定义与取值
来源：http://ind.hammf.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xdv.ctjpmb.com

[R18] 遍历数组
来源：http://smm.sysykeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mfz.yonumen.top

[R19] 数组长度
来源：http://jcs.ehwqpu.com

echo "${#arr[@]}"
来源：http://nsf.bbcook.cn

[R20] 关联数组（字典）
来源：http://xwl.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pqj.vqdsnc.cn

[R21] 字符串长度
来源：http://xwn.gaohongyu789.top

echo "${#s}"
来源：http://ejw.guannengcc.top

[R22] 截取子串
来源：http://wdi.cheryme.top

echo "${s:0:5}"
来源：http://txo.tian-w.cn

[R23] 字符串替换
来源：http://kly.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jzx.xziqi.cn

[R24] 大小写转换
来源：http://jej.xuanzx.com

echo "${s^^}"; echo "${s,,}"
来源：http://ppf.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://pwo.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ybm.fktsv.cn

[R26] 命令替换
来源：http://qnl.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://noc.jlsjyb.cn

[R27] 算术展开
来源：http://brm.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://aea.hysaishi.cn

[R28] 浮点运算
来源：http://pjf.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://apu.wangshuangyany.cn

[R29] 定义函数
来源：http://ozx.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gkq.snrcjt.cn

[R30] 函数返回状态码
来源：http://toz.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://vyo.tianlin.xyz

[R31] 局部变量
来源：http://xqk.shanyushiyangtech.top

f() { local x=1; echo "$x"; }
来源：http://bew.yuanzhike.top

[R32] 参数个数校验
来源：http://eku.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mmn.gzhubu.top

[R33] 捕获错误并提示行号
来源：http://fqx.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qii.sxryk.cn

[R34] 退出时清理
来源：http://lwh.yj20258.top

trap 'rm -f "$tmp"' EXIT
来源：http://qon.gzhubu.top

[R35] 后台执行并等待
来源：http://pmk.ybcxt.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wmb.hysaishi.cn

[R36] 并发执行多个任务
来源：http://bfc.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uas.hnqzz.top

[R37] 把输出赋给变量
来源：http://kkf.fengsongda.top

files=$(ls -1)
来源：http://kyj.fktsv.cn

[R38] 管道串联
来源：http://zkr.gotoacloud.top

cat a.txt | grep -i error | wc -l
来源：http://gwx.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://zhz.redwolf501.top

cmd > out.log 2>&1
来源：http://aps.havefunace.top

[R40] 追加写日志
来源：http://fup.chenzaomai.com

echo "log" >> out.log
来源：http://yif.chenlongwang.top

[R41] 丢弃输出
来源：http://txg.vehdjk.com

cmd >/dev/null 2>&1
来源：http://rru.xziqi.cn

[R42] 输入重定向
来源：http://jgo.jinqigfzy.top

wc -l < a.txt
来源：http://zys.zhaomingkeji.xyz

[R43] 按名字查找文件
来源：http://ttr.daxiang520.top

find . -name "*.log" -type f
来源：http://evx.cdnleiting.top

[R44] 按修改时间查找
来源：http://lpz.cashguo.top

find . -mtime -7 -type f
来源：http://mwr.xuetiantiany.cn

[R45] 批量删除
来源：http://igk.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://isk.dianchejie.cn

[R46] 递归替换文件内容
来源：http://hid.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fta.zhoulong.xyz

[R47] sed 单行替换
来源：http://fss.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://vzt.daxiang520.top

[R48] awk 取指定列
来源：http://cyh.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://wrb.jinqigfzy.top

[R49] awk 带条件
来源：http://xup.andypj.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tfa.yonumen.top

[R50] awk 求和
来源：http://ewt.yj20258.top

awk '{s += $2} END {print s}' a.txt
来源：http://ohm.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://fqy.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://chq.aizwys.cn

[R52] 统计行数
来源：http://wle.yangfankeji.com

wc -l a.txt
来源：http://inq.zhaomingkeji.xyz

[R53] 查看文件头与实时尾
来源：http://wkb.jqgfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rgm.sweek.top

[R54] 比较两个文件
来源：http://wtj.zhiwuduotai.top

diff a.txt b.txt
来源：http://sjz.shanyushiyangkeji.top

[R55] 压缩与解压
来源：http://pfc.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mgu.cashguo.top

[R56] 远程拷贝
来源：http://owi.cdnleiting.top

scp file user@host:/path/
来源：http://mtw.uphjek.com

[R57] 远程执行命令
来源：http://uxo.andypj.xyz

ssh user@host 'uptime'
来源：http://sjp.shuidangran.top

[R58] 下载文件
来源：http://kfl.jinqigufen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qwa.sxryk.cn

[R59] 发 POST JSON
来源：http://sss.meibo888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://alg.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://gkt.yj20258.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tzd.tianlin.xyz

[R61] 磁盘占用
来源：http://sgr.jlsjyb.cn

df -h;  du -sh *
来源：http://ajt.ppjwa.cn

[R62] 找最占空间的文件
来源：http://zib.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://akz.yueranfly.top

[R63] 内存与进程
来源：http://hqx.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://sxv.shangyingyoupin.top

[R64] 结束进程
来源：http://fjx.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://cam.yongpay.top

[R65] 查看端口占用
来源：http://kyw.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mqn.ydzc1.top

[R66] 定时任务
来源：http://cmu.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://nuv.yangfankeji.com

[R67] 生成随机十六进制串
来源：http://kif.ehwqpu.com

openssl rand -hex 16
来源：http://nxn.meibo888.top

[R68] 计算文件校验值
来源：http://oxv.fktsv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gtt.hfpthk.cn

[R69] 生成随机密码
来源：http://aoy.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://mzj.tian-w.cn

[R70] 时间戳与互转
来源：http://bnw.sweek.top

date +%s;  date -d @1700000000
来源：http://xlq.shuidangran.top

[R71] 日期格式化
来源：http://pic.xylfe.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eot.kuanghao11.cn

[R72] 等待端口就绪
来源：http://may.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gzk.hywenlv.cn

[R73] 分割大日志
来源：http://rxv.jlsjyb.cn

split -l 1000 big.log part_
来源：http://gfh.redwolf501.top

[R74] 批量重命名
来源：http://eeo.yj20258.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://app.sxryk.cn

[R75] 导出环境变量
来源：http://iqj.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://nmy.9152youxi.cn

[R76] 使用临时文件
来源：http://ldz.zhongyouzk.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tul.ydzc1.top

[R77] 读取用户输入
来源：http://gia.sysykeji.top

read -rp "请输入: " ans
来源：http://uog.hnxiangtu.top

[R78] 交互式菜单
来源：http://naf.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://swt.tianlin.xyz

[R79] 解析命令行选项
来源：http://byn.wangdashe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qdv.0kj1m.cn

[R80] 查看脚本执行耗时
来源：http://cxg.yangfankeji.com

time ./run.sh
来源：http://asi.bbcook.cn

================================================================================
来源：http://xru.andypj.xyz

S. C / C++ 专题
来源：http://kuw.hcnkem.com

================================================================================
来源：http://apl.zhongyouzk.top

[S01] C：Hello World
来源：http://kge.epnwcf.com

#include <stdio.h>
来源：http://cvp.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zhb.sjlbkw.cn

[S02] C：变量与格式化输出
来源：http://sbi.ybcxt.top

int a = 10; printf("%d\n", a);
来源：http://zwd.0kj1m.cn

[S03] C：读入整数
来源：http://sea.zdbjq.cn

int x; scanf("%d", &x);
来源：http://xim.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://vek.hcnkem.com

char dst[32]; strcpy(dst, "hi");
来源：http://wqx.yj20258888.top

[S05] C：字符串长度
来源：http://txd.ctjpmb.com

strlen(s)
来源：http://abb.zhixingplan.top

[S06] C：字符串比较
来源：http://til.yanxiufei.cn

strcmp(a, b) == 0
来源：http://cvw.ctjpmb.com

[S07] C：数组遍历求和
来源：http://zms.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yvi.pycfn.com

[S08] C：动态内存分配与释放
来源：http://ftg.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mbf.cheryme.top

[S09] C：结构体定义与初始化
来源：http://rlz.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gxo.vqdsnc.cn

[S10] C：指针与解引用
来源：http://kia.jqgufenzy.top

int *p = &a;  *p = 5;
来源：http://suk.sysykeji.top

[S11] C：逐行读文件
来源：http://hxj.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://zkn.jiagoushi.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://amc.zdqjudy.top

fclose(f);
来源：http://nxr.mhx1999.top

[S12] C：写文件
来源：http://psf.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wjt.daria6918.cn

[S13] C：宏定义
来源：http://nxj.yj20258.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qdh.kuanghao11.cn

[S14] C：枚举
来源：http://vlz.epnwcf.com

enum Color { RED, GREEN, BLUE };
来源：http://vir.feifeiyinyue.top

[S15] C：类型转换
来源：http://oap.ybcxt.top

(double) a / b
来源：http://xqx.gogol.net.cn

[S16] C：位操作置位
来源：http://wdp.yanxiufei.cn

x |= (1 << 3);
来源：http://pju.nwbrower.top

[S17] C：安全拼接字符串
来源：http://rsy.zhongyouzk.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cde.sufxvd.cn

[S18] C：命令行参数
来源：http://pys.smart0.xyz

int main(int argc, char **argv)
来源：http://rpd.chenjidiqi.icu

[S19] C：快速排序
来源：http://fjg.vehdjk.com

qsort(a, n, sizeof(int), cmp);
来源：http://lvh.hnqzz.top

[S20] C：二分查找
来源：http://hzy.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://izi.nanxuanxn.top

[S21] C：字符类别判断
来源：http://mma.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yat.epnwcf.com

[S22] C：字符串转数字
来源：http://pax.uphjek.com

atoi("42");  strtod("3.14", NULL);
来源：http://xwr.cashguo.top

[S23] C：随机数
来源：http://vci.zhongyouzk.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oxi.yonumen.top

[S24] C：获取本地时间
来源：http://kna.xuanzx.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://not.vqdsnc.cn

[S25] C：内存拷贝
来源：http://oot.zdqjudy.top

memcpy(dst, src, n);
来源：http://kht.gotoacloud.top

[S26] C：内存清零
来源：http://dbb.fzhhl.top

memset(a, 0, sizeof a);
来源：http://gyf.hongshengwenyu.top

[S27] C：定义常量
来源：http://okm.xingfuxueyuan.xyz

const double PI = 3.14159;
来源：http://sdw.yangfankeji.com

[S28] C：静态变量
来源：http://rps.tarul.cn

static int counter = 0;
来源：http://ibc.cucudq.cn

[S29] C：变参函数
来源：http://fli.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gui.hnxiangtu.top

[S30] C：头文件保护
来源：http://ixo.daxiang520.top

#ifndef X_H
来源：http://uwk.hnqzz.top

#define X_H
来源：http://xyl.svipenyu.cn

#endif
来源：http://pwy.guowangkeji.top

[S31] C++：Hello World
来源：http://xnd.fehbvm.com

#include <iostream>
来源：http://mqp.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://yci.chenlongwang.top

[S32] C++：字符串
来源：http://hkw.birdmap.top

std::string s = "hi";  s += "!";
来源：http://vav.daxiang520.top

[S33] C++：vector 增删
来源：http://qtl.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uwn.yongpay.top

[S34] C++：遍历 vector
来源：http://bqw.ywan-chungtsiang.top

for (auto &x : v) { std::cout << x; }
来源：http://eoq.ehwqpu.com

[S35] C++：map
来源：http://vwx.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vxf.zhoulong.xyz

[S36] C++：unordered_map
来源：http://tqk.zdbjq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fsg.yj20258.top

[S37] C++：set
来源：http://qfg.chenlongwang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nor.9152youxi.cn

[S38] C++：排序
来源：http://atr.birdmap.top

std::sort(v.begin(), v.end());
来源：http://gre.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://uql.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mof.daria6918.cn

[S40] C++：查找元素
来源：http://efb.nanxuanxn.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cny.meibo888.top

[S41] C++：类与构造函数
来源：http://ydl.mhx1999.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mbj.shuidangran.top

[S42] C++：继承与虚函数
来源：http://ppy.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://ssu.9152youxi.cn

[S43] C++：智能指针
来源：http://bis.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://mzx.daria6918.cn

[S44] C++：引用传参
来源：http://eto.daria6918.cn

void inc(int &x) { ++x; }
来源：http://oxf.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://qrg.cashguo.top

auto add = [](int a, int b) { return a + b; };
来源：http://qbk.redwolf501.top

[S46] C++：函数模板
来源：http://gfa.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eqg.snrcjt.cn

[S47] C++：结构化绑定遍历
来源：http://jgz.hysaishi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wxd.chenzaomai.com

[S48] C++：逐行读文件
来源：http://lcm.quarkkingdee.top

std::ifstream in("a.txt");  std::string line;
来源：http://bvp.pycfn.com

while (std::getline(in, line)) { }
来源：http://yvf.chenlongwang.top

[S49] C++：写文件
来源：http://ptc.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eni.dashuyun.cn

[S50] C++：格式化数字
来源：http://lqz.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aqn.tian-w.cn

[S51] C++：显式类型转换
来源：http://evq.xuanzx.com

static_cast<double>(a) / b
来源：http://zks.cheryme.top

[S52] C++：const 与 noexcept
来源：http://jrv.jqgfzy.top

int size() const noexcept { return n_; }
来源：http://ikm.jqgfzy.top

[S53] C++：移动语义
来源：http://wwl.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://ncr.hammf.cn

[S54] C++：异常处理
来源：http://nfv.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bfo.yueranfly.top

[S55] C++：结构化绑定
来源：http://bis.yongpay.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nuw.sjlbkw.cn

[S56] C++：optional
来源：http://eqf.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://azr.ctjpmb.com

[S57] C++：编译期常量
来源：http://ndl.hnqzz.top

constexpr int N = 10;
来源：http://gcf.daria6918.cn

[S58] C++：命名空间
来源：http://uyw.hcnkem.com

namespace ns { int f() { return 1; } }
来源：http://icz.aizwys.cn

[S59] C++：静态断言
来源：http://wtw.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vqy.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://voq.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://npq.fehbvm.com

================================================================================
来源：http://kvj.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ppq.yangfankeji.com

================================================================================
来源：http://wiz.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://szc.yonumen.top

println("Hello")
来源：http://cec.nanxinkj.top

[T02] Kotlin：变量
来源：http://bom.xingfuxueyuan.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://edk.jqgfzy.top

[T03] Kotlin：字符串模板
来源：http://zqn.hcnkem.com

"值: $b"
来源：http://tql.yonumen.top

[T04] Kotlin：空安全
来源：http://xef.hesvh.cn

val n: String? = null;  n?.length
来源：http://mhl.hywenlv.cn


<!-- 参考信息 -->