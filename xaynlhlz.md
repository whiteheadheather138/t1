代发 wailian999

name="${1:-default}"
来源：http://oek.ehwqpu.com

[R06] 判断命令是否存在
来源：http://tny.wangdashe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vze.jqgufenzy.top

[R07] if 判断文件
来源：http://vur.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jqh.jqgufenzy.top

[R08] 数值比较
来源：http://bue.sysykeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vda.52xcode.cn

[R09] 字符串比较
来源：http://bgj.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rxn.hesvh.cn

[R10] 正则匹配
来源：http://ubt.mhx1999.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nkj.fehbvm.com

[R11] case 多分支
来源：http://nyh.cashguo.top

case "$1" in
来源：http://seu.xuetiantiany.cn

start) echo "启动" ;;
来源：http://abm.0kj1m.cn

stop)  echo "停止" ;;
来源：http://bkz.tian-w.cn

*)     echo "未知命令" ;;
来源：http://toz.9152youxi.cn

esac
来源：http://zxt.yvedp.cn

[R12] for 遍历文件
来源：http://jyc.vehdjk.com

for f in *.txt; do echo "$f"; done
来源：http://dsl.pengpengdd.cyou

[R13] for 计数循环
来源：http://rhi.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://kdm.shanyushiyangkeji.top

[R14] C 风格 for
来源：http://pmt.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xaz.ivvv.top

[R15] while 逐行读文件
来源：http://rrb.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://str.hesvh.cn

[R16] until 等待条件
来源：http://vun.havefunace.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ebk.sxryk.cn

[R17] 数组定义与取值
来源：http://zoc.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://wry.hfpthk.cn

[R18] 遍历数组
来源：http://szb.zdqjudy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nab.zhaomingkeji.xyz

[R19] 数组长度
来源：http://cga.yongpay.top

echo "${#arr[@]}"
来源：http://pdg.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://goe.cqqwz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://chr.hnxiangtu.top

[R21] 字符串长度
来源：http://lvd.gogol.net.cn

echo "${#s}"
来源：http://tvu.yvedp.cn

[R22] 截取子串
来源：http://mjw.redwolf501.top

echo "${s:0:5}"
来源：http://gjs.sxryk.cn

[R23] 字符串替换
来源：http://jxe.birdmap.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eud.0kj1m.cn

[R24] 大小写转换
来源：http://qot.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://sfh.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://wjl.zdqjudy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ipb.xziqi.cn

[R26] 命令替换
来源：http://phg.fzhhl.top

now=$(date +%F); echo "$now"
来源：http://kcq.ydzc1.top

[R27] 算术展开
来源：http://fky.fengsongda.top

echo $((1 + 2 * 3))
来源：http://ogb.aizwys.cn

[R28] 浮点运算
来源：http://lhp.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://coe.ybcxt.top

[R29] 定义函数
来源：http://mmg.yuanzhike.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jws.feifeiyinyue.top

[R30] 函数返回状态码
来源：http://ggj.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://mgm.dianchejie.cn

[R31] 局部变量
来源：http://jvw.9152youxi.cn

f() { local x=1; echo "$x"; }
来源：http://fhj.hesvh.cn

[R32] 参数个数校验
来源：http://fob.hnqzz.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pxp.yfazqb.com

[R33] 捕获错误并提示行号
来源：http://lew.kuanghao11.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qts.sxryk.cn

[R34] 退出时清理
来源：http://qri.redwolf501.top

trap 'rm -f "$tmp"' EXIT
来源：http://ybw.ivvv.top

[R35] 后台执行并等待
来源：http://sps.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gia.quarkkingdee.top

[R36] 并发执行多个任务
来源：http://pbf.daxiang520.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ipf.zhixingplan.top

[R37] 把输出赋给变量
来源：http://rzt.jinqigufen.top

files=$(ls -1)
来源：http://hdr.chenjidiqi.icu

[R38] 管道串联
来源：http://klq.cucudq.cn

cat a.txt | grep -i error | wc -l
来源：http://jhq.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://hbc.jinghuilouyu.cn

cmd > out.log 2>&1
来源：http://qnw.ivvv.top

[R40] 追加写日志
来源：http://zkb.aibaodan.cn

echo "log" >> out.log
来源：http://nsh.cashguo.top

[R41] 丢弃输出
来源：http://lru.xziqi.cn

cmd >/dev/null 2>&1
来源：http://rpr.tarul.cn

[R42] 输入重定向
来源：http://tpm.yuanzhike.top

wc -l < a.txt
来源：http://fof.vehdjk.com

[R43] 按名字查找文件
来源：http://axu.zhaomingkeji.xyz

find . -name "*.log" -type f
来源：http://glw.52xcode.cn

[R44] 按修改时间查找
来源：http://mhn.dashuyun.cn

find . -mtime -7 -type f
来源：http://lmf.yangfankeji.com

[R45] 批量删除
来源：http://pok.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://tjh.daxiang520.top

[R46] 递归替换文件内容
来源：http://xma.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yvd.daxiang520.top

[R47] sed 单行替换
来源：http://zqn.yonumen.top

sed -i 's/foo/bar/g' a.txt
来源：http://rgz.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://wya.fzhhl.top

awk '{print $1, $3}' a.txt
来源：http://ddr.ydjk.org.cn

[R49] awk 带条件
来源：http://igw.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://efa.yueranfly.top

[R50] awk 求和
来源：http://vpo.tian-w.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zxb.sweek.top

[R51] 排序去重取前几
来源：http://kyh.mhx1999.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rhn.nwbrower.top

[R52] 统计行数
来源：http://hyj.cqqwz.cn

wc -l a.txt
来源：http://fdz.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://eyx.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oow.daria6918.cn

[R54] 比较两个文件
来源：http://qbt.shuidangran.top

diff a.txt b.txt
来源：http://lts.yuxming.cn

[R55] 压缩与解压
来源：http://bab.gzhubu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yaj.kuanghao11.cn

[R56] 远程拷贝
来源：http://ytn.chenzaomai.com

scp file user@host:/path/
来源：http://dxn.yuxming.cn

[R57] 远程执行命令
来源：http://wog.tarul.cn

ssh user@host 'uptime'
来源：http://yrv.chenlongwang.top

[R58] 下载文件
来源：http://err.yanxiufei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://elz.chenlongwang.top

[R59] 发 POST JSON
来源：http://wpy.fengsongda.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ytg.hfpthk.cn

[R60] 只看 HTTP 状态码
来源：http://iic.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pmo.zhongyouzk.top

[R61] 磁盘占用
来源：http://ekh.zhijiandao.cn

df -h;  du -sh *
来源：http://dgi.yvedp.cn

[R62] 找最占空间的文件
来源：http://onj.vehdjk.com

du -ah . | sort -rh | head -10
来源：http://loz.aibaodan.cn

[R63] 内存与进程
来源：http://puz.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://tyc.jinqigfzy.top

[R64] 结束进程
来源：http://meo.chenlongwang.top

kill -9 $(pgrep -f app.py)
来源：http://tge.bjfxy.top

[R65] 查看端口占用
来源：http://gkd.ydzc1.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gxj.shuidangran.top

[R66] 定时任务
来源：http://crs.yanxiufei.cn

crontab -e;  crontab -l
来源：http://fpt.aibaodan.cn

[R67] 生成随机十六进制串
来源：http://mtm.jlsjyb.cn

openssl rand -hex 16
来源：http://bhz.yanxiufei.cn

[R68] 计算文件校验值
来源：http://veq.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://ciu.snrcjt.cn

[R69] 生成随机密码
来源：http://jcd.meibo888.top

head -c 16 /dev/urandom | base64
来源：http://ndw.andypj.xyz

[R70] 时间戳与互转
来源：http://hdz.c1oappe.top

date +%s;  date -d @1700000000
来源：http://cuh.zhengqikj.top

[R71] 日期格式化
来源：http://rcg.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://soa.yj20258.top

[R72] 等待端口就绪
来源：http://acu.jiagoushi.top

until nc -z localhost 3306; do sleep 1; done
来源：http://tpt.pycfn.com

[R73] 分割大日志
来源：http://cvy.ydjk.org.cn

split -l 1000 big.log part_
来源：http://tcs.hfpthk.cn

[R74] 批量重命名
来源：http://kus.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bhq.zhengqikj.top

[R75] 导出环境变量
来源：http://ylr.fengsongda.top

export PATH="$HOME/bin:$PATH"
来源：http://uhc.zhoulong.xyz

[R76] 使用临时文件
来源：http://thp.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oey.cashguo.top

[R77] 读取用户输入
来源：http://jge.dashuyun.cn

read -rp "请输入: " ans
来源：http://gyv.daria6918.cn

[R78] 交互式菜单
来源：http://nki.zhaomingkeji.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://tle.tanke756.top

[R79] 解析命令行选项
来源：http://nbu.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ext.birdmap.top

[R80] 查看脚本执行耗时
来源：http://frl.zhiwuduotai.top

time ./run.sh
来源：http://bzg.52xcode.cn

================================================================================
来源：http://ubx.snrcjt.cn

S. C / C++ 专题
来源：http://art.shuidangran.top

================================================================================
来源：http://foa.vehdjk.com

[S01] C：Hello World
来源：http://jpq.jyoumei.cn

#include <stdio.h>
来源：http://vio.aizwys.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hxc.vehdjk.com

[S02] C：变量与格式化输出
来源：http://mgo.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://evr.svipenyu.cn

[S03] C：读入整数
来源：http://ega.hfpthk.cn

int x; scanf("%d", &x);
来源：http://cjb.hnqzz.top

[S04] C：字符串复制
来源：http://vyg.birdmap.top

char dst[32]; strcpy(dst, "hi");
来源：http://hyo.hammf.cn

[S05] C：字符串长度
来源：http://qos.aizwys.cn

strlen(s)
来源：http://jwe.dianchejie.cn

[S06] C：字符串比较
来源：http://svd.shuidangran.top

strcmp(a, b) == 0
来源：http://dmf.chenlongwang.top

[S07] C：数组遍历求和
来源：http://uwi.redwolf501.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dqs.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://xfp.yj20258.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tkc.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://ias.daxiang520.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ldy.52xcode.cn

[S10] C：指针与解引用
来源：http://dcz.gotoacloud.top

int *p = &a;  *p = 5;
来源：http://dpv.c1oappe.top

[S11] C：逐行读文件
来源：http://oga.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://uty.fehbvm.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://vvx.zhengqikj.top

fclose(f);
来源：http://krf.sysykeji.top

[S12] C：写文件
来源：http://fto.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gvz.chenlongwang.top

[S13] C：宏定义
来源：http://zis.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hct.guannengcc.top

[S14] C：枚举
来源：http://ttp.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://wvq.shzxlz.cn

[S15] C：类型转换
来源：http://cyh.yuxming.cn

(double) a / b
来源：http://ybg.redwolf501.top

[S16] C：位操作置位
来源：http://kwm.chenlongwang.top

x |= (1 << 3);
来源：http://yyv.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://ebe.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://drx.iojbl.cn

[S18] C：命令行参数
来源：http://vfi.zdqjudy.top

int main(int argc, char **argv)
来源：http://igr.zhixingplan.top

[S19] C：快速排序
来源：http://rom.hesvh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vnt.nanxinkj.top

[S20] C：二分查找
来源：http://acx.kuanghao11.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fqc.shuidangran.top

[S21] C：字符类别判断
来源：http://qza.hnqzz.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fgy.shzxlz.cn

[S22] C：字符串转数字
来源：http://pni.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://rnz.gzhubu.top

[S23] C：随机数
来源：http://msr.nwbrower.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jpe.fehbvm.com

[S24] C：获取本地时间
来源：http://xmv.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yol.yangfankeji.com

[S25] C：内存拷贝
来源：http://hap.jianghu66.top

memcpy(dst, src, n);
来源：http://jfj.yonumen.top

[S26] C：内存清零
来源：http://fuj.daxiang520.top

memset(a, 0, sizeof a);
来源：http://cyc.hesvh.cn

[S27] C：定义常量
来源：http://vmh.ctjpmb.com

const double PI = 3.14159;
来源：http://jli.nanxinkj.top

[S28] C：静态变量
来源：http://tjc.dashuyun.cn

static int counter = 0;
来源：http://gyp.havefunace.top

[S29] C：变参函数
来源：http://dpm.nanxinkj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ylv.fktsv.cn

[S30] C：头文件保护
来源：http://tzf.tanke756.top

#ifndef X_H
来源：http://jxt.hcnkem.com

#define X_H
来源：http://pfx.redwolf501.top

#endif
来源：http://yuy.cashguo.top

[S31] C++：Hello World
来源：http://zbr.gotoacloud.top

#include <iostream>
来源：http://ufn.nanxuanxn.top

int main() { std::cout << "Hello\n"; }
来源：http://fxe.dashuyun.cn

[S32] C++：字符串
来源：http://vnv.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://ljh.jlsjyb.cn

[S33] C++：vector 增删
来源：http://jra.pycfn.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sbm.fengsongda.top

[S34] C++：遍历 vector
来源：http://bhr.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://eqs.hywenlv.cn

[S35] C++：map
来源：http://qin.xingfuxueyuan.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fue.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://zbk.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bbd.yanxiufei.cn

[S37] C++：set
来源：http://dwb.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://znf.kuanghao11.cn

[S38] C++：排序
来源：http://zzd.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://nej.dashuyun.cn

[S39] C++：自定义比较器排序
来源：http://fad.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jbs.zhengqikj.top

[S40] C++：查找元素
来源：http://unj.pycfn.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dtb.0kj1m.cn

[S41] C++：类与构造函数
来源：http://cyp.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yqy.xziqi.cn

[S42] C++：继承与虚函数
来源：http://gpv.pycfn.com

class B : public Base { public: void f() override {} };
来源：http://fnb.haohaochexian.top

[S43] C++：智能指针
来源：http://lqs.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://fsu.svipenyu.cn

[S44] C++：引用传参
来源：http://nrg.fktsv.cn

void inc(int &x) { ++x; }
来源：http://mvh.ybcxt.top

[S45] C++：lambda
来源：http://ztk.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://paq.gotoacloud.top

[S46] C++：函数模板
来源：http://dhk.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fik.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://okb.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eso.haohaochexian.top

[S48] C++：逐行读文件
来源：http://xtx.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://yes.cashguo.top

while (std::getline(in, line)) { }
来源：http://ysz.xylfe.cn

[S49] C++：写文件
来源：http://nhx.quarkkingdee.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yjk.sweek.top

[S50] C++：格式化数字
来源：http://znh.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zun.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://cgo.jinqigfzy.top

static_cast<double>(a) / b
来源：http://ene.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://nmg.jinqigfzy.top

int size() const noexcept { return n_; }
来源：http://rsq.sweek.top

[S53] C++：移动语义
来源：http://ngr.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://zny.aibaodan.cn

[S54] C++：异常处理
来源：http://sar.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://itg.fehbvm.com

[S55] C++：结构化绑定
来源：http://chk.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hvn.bjfxy.top

[S56] C++：optional
来源：http://qps.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xsc.mhx1999.top

[S57] C++：编译期常量
来源：http://ehh.hcnkem.com

constexpr int N = 10;
来源：http://hgx.smart0.xyz

[S58] C++：命名空间
来源：http://rux.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://giw.hcnkem.com

[S59] C++：静态断言
来源：http://ksy.redwolf501.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ulj.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://eds.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oex.meibo888.top

================================================================================
来源：http://wzq.zdqjudy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://szd.daria6918.cn

================================================================================
来源：http://gkf.fktsv.cn

[T01] Kotlin：Hello World
来源：http://jki.jinqigufen.top

println("Hello")
来源：http://nah.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://mot.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dsx.zhixingplan.top

[T03] Kotlin：字符串模板
来源：http://udq.daria6918.cn

"值: $b"
来源：http://mbt.xuanzx.com

[T04] Kotlin：空安全
来源：http://mvp.yvedp.cn

val n: String? = null;  n?.length
来源：http://lek.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://qsm.smart0.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rwb.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://vdj.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eik.xinyue.icu


<!-- 参考信息 -->