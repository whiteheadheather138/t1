代发 wailian999

name="${1:-default}"
来源：http://ign.zhengqikj.top

[R06] 判断命令是否存在
来源：http://awz.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zwf.daria6918.cn

[R07] if 判断文件
来源：http://fwu.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cep.zhengqikj.top

[R08] 数值比较
来源：http://lws.chenlongwang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pov.tian-w.cn

[R09] 字符串比较
来源：http://hgn.nwbrower.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mnj.feifeiyinyue.top

[R10] 正则匹配
来源：http://csk.andypj.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mdr.daxiang520.top

[R11] case 多分支
来源：http://nee.xingfuxueyuan.xyz

case "$1" in
来源：http://gaf.yvedp.cn

start) echo "启动" ;;
来源：http://qjw.jianghu66.top

stop)  echo "停止" ;;
来源：http://jhx.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://waj.hongshengwenyu.top

esac
来源：http://ccp.feifeiyinyue.top

[R12] for 遍历文件
来源：http://umi.ydzc1.top

for f in *.txt; do echo "$f"; done
来源：http://ege.nanxinkj.top

[R13] for 计数循环
来源：http://zda.sweek.top

for i in {1..10}; do echo "$i"; done
来源：http://kfl.quarkkingdee.top

[R14] C 风格 for
来源：http://ifb.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tqq.dianchejie.cn

[R15] while 逐行读文件
来源：http://xue.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nvr.zhiwuduotai.top

[R16] until 等待条件
来源：http://joq.hnqzz.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lkc.havefunace.top

[R17] 数组定义与取值
来源：http://wwt.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://bkc.jinghuilouyu.cn

[R18] 遍历数组
来源：http://ivv.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rzl.jinyuanbaomall.cn

[R19] 数组长度
来源：http://wci.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://xtg.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://ufw.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dno.quarkkingdee.top

[R21] 字符串长度
来源：http://vqh.jlsjyb.cn

echo "${#s}"
来源：http://mlg.andypj.xyz

[R22] 截取子串
来源：http://vag.hammf.cn

echo "${s:0:5}"
来源：http://ueh.daxiang520.top

[R23] 字符串替换
来源：http://vlg.zdqjudy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rhd.xuanzx.com

[R24] 大小写转换
来源：http://sqj.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nhk.kuanghao11.cn

[R25] 去后缀 / 去前缀
来源：http://eiu.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://eze.hnxiangtu.top

[R26] 命令替换
来源：http://adj.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://qoh.zhoulong.xyz

[R27] 算术展开
来源：http://yoq.svipenyu.cn

echo $((1 + 2 * 3))
来源：http://jdp.wangdashe.top

[R28] 浮点运算
来源：http://jaf.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://iqy.c1oappe.top

[R29] 定义函数
来源：http://xft.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qug.guowangkeji.top

[R30] 函数返回状态码
来源：http://opv.cqqwz.cn

f() { return 0; }; f || echo "失败了"
来源：http://evw.xingfuxueyuan.xyz

[R31] 局部变量
来源：http://xjl.aibaodan.cn

f() { local x=1; echo "$x"; }
来源：http://qtn.xingfuxueyuan.xyz

[R32] 参数个数校验
来源：http://zic.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hpx.nanxuanxn.top

[R33] 捕获错误并提示行号
来源：http://tio.redwolf501.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://izl.vqdsnc.cn

[R34] 退出时清理
来源：http://sgg.mhx1999.top

trap 'rm -f "$tmp"' EXIT
来源：http://fwe.fzhhl.top

[R35] 后台执行并等待
来源：http://xst.iojbl.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mwd.cucudq.cn

[R36] 并发执行多个任务
来源：http://lrv.tian-w.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gke.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://tvb.hnqzz.top

files=$(ls -1)
来源：http://fyf.hesvh.cn

[R38] 管道串联
来源：http://iqg.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://hpw.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://gns.xuanzx.com

cmd > out.log 2>&1
来源：http://rmj.fanxiaobao.xyz

[R40] 追加写日志
来源：http://ikv.shuidangran.top

echo "log" >> out.log
来源：http://htf.fehbvm.com

[R41] 丢弃输出
来源：http://fxd.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://lqw.0kj1m.cn

[R42] 输入重定向
来源：http://rqe.yuanzhike.top

wc -l < a.txt
来源：http://dtl.zhongyouzk.top

[R43] 按名字查找文件
来源：http://kaq.yj20258.top

find . -name "*.log" -type f
来源：http://elf.sweek.top

[R44] 按修改时间查找
来源：http://bax.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://yhs.yueranfly.top

[R45] 批量删除
来源：http://gdj.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://etl.yuxming.cn

[R46] 递归替换文件内容
来源：http://xwz.ydjk.org.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ovp.fktsv.cn

[R47] sed 单行替换
来源：http://quh.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://our.vehdjk.com

[R48] awk 取指定列
来源：http://gnp.daxiang520.top

awk '{print $1, $3}' a.txt
来源：http://jzl.pengpengdd.cyou

[R49] awk 带条件
来源：http://vri.aizwys.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wlb.vehdjk.com

[R50] awk 求和
来源：http://dbc.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://gdq.ybcxt.top

[R51] 排序去重取前几
来源：http://stv.yj20258888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://esm.smart0.xyz

[R52] 统计行数
来源：http://kiy.xinyue.icu

wc -l a.txt
来源：http://zsr.pycfn.com

[R53] 查看文件头与实时尾
来源：http://bly.ivvv.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aet.xinyue.icu

[R54] 比较两个文件
来源：http://jsq.tanke756.top

diff a.txt b.txt
来源：http://aqm.ydjk.org.cn

[R55] 压缩与解压
来源：http://dwf.mhx1999.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zdc.0kj1m.cn

[R56] 远程拷贝
来源：http://wmq.guowangkeji.top

scp file user@host:/path/
来源：http://slv.yueranfly.top

[R57] 远程执行命令
来源：http://jwe.zhengqikj.top

ssh user@host 'uptime'
来源：http://kbv.kuanghao11.cn

[R58] 下载文件
来源：http://mim.tarul.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hli.aibaodan.cn

[R59] 发 POST JSON
来源：http://oys.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tih.fehbvm.com

[R60] 只看 HTTP 状态码
来源：http://kxq.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mqb.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://gny.ywan-chungtsiang.top

df -h;  du -sh *
来源：http://ton.yj20258.top

[R62] 找最占空间的文件
来源：http://dpv.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://mjc.kuanghao11.cn

[R63] 内存与进程
来源：http://cqg.havefunace.top

free -h;  ps aux | grep nginx
来源：http://cyw.jiagoushi.top

[R64] 结束进程
来源：http://ldo.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://zyx.pycfn.com

[R65] 查看端口占用
来源：http://ldv.hfpthk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mdo.zhengqikj.top

[R66] 定时任务
来源：http://wyn.tarul.cn

crontab -e;  crontab -l
来源：http://erc.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://bum.ivvv.top

openssl rand -hex 16
来源：http://rqt.52xcode.cn

[R68] 计算文件校验值
来源：http://tqb.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xei.ywan-chungtsiang.top

[R69] 生成随机密码
来源：http://syj.jinqigufen.top

head -c 16 /dev/urandom | base64
来源：http://rjf.chenzaomai.com

[R70] 时间戳与互转
来源：http://rza.yonumen.top

date +%s;  date -d @1700000000
来源：http://akz.svipenyu.cn

[R71] 日期格式化
来源：http://kno.zhongyouzk.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zsd.ydzc1.top

[R72] 等待端口就绪
来源：http://aoi.shanyushiyangtech.top

until nc -z localhost 3306; do sleep 1; done
来源：http://eep.aizwys.cn

[R73] 分割大日志
来源：http://rex.redwolf501.top

split -l 1000 big.log part_
来源：http://upq.havefunace.top

[R74] 批量重命名
来源：http://tbx.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uwg.hongshengwenyu.top

[R75] 导出环境变量
来源：http://mwe.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://gbk.jianghu66.top

[R76] 使用临时文件
来源：http://yto.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vkg.snrcjt.cn

[R77] 读取用户输入
来源：http://pte.kuanghao11.cn

read -rp "请输入: " ans
来源：http://bpi.snrcjt.cn

[R78] 交互式菜单
来源：http://bnb.bjfxy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uyi.chenlongwang.top

[R79] 解析命令行选项
来源：http://emn.sxryk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zos.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://fvq.smart0.xyz

time ./run.sh
来源：http://lta.shuidangran.top

================================================================================
来源：http://bwp.aizwys.cn

S. C / C++ 专题
来源：http://zli.fzhhl.top

================================================================================
来源：http://axi.aizwys.cn

[S01] C：Hello World
来源：http://lfc.yuxming.cn

#include <stdio.h>
来源：http://dmv.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://llb.uphjek.com

[S02] C：变量与格式化输出
来源：http://hwm.yuxming.cn

int a = 10; printf("%d\n", a);
来源：http://nhn.dianchejie.cn

[S03] C：读入整数
来源：http://aeb.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://cfc.tanke756.top

[S04] C：字符串复制
来源：http://jwd.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://tpt.fehbvm.com

[S05] C：字符串长度
来源：http://eea.jlsjyb.cn

strlen(s)
来源：http://rmj.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://jwy.jlsjyb.cn

strcmp(a, b) == 0
来源：http://ihy.0kj1m.cn

[S07] C：数组遍历求和
来源：http://nry.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hpq.ybcxt.top

[S08] C：动态内存分配与释放
来源：http://wjl.wangshuangyany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nxd.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://xfr.0kj1m.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sza.9152youxi.cn

[S10] C：指针与解引用
来源：http://ztm.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://phv.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://vra.tanke756.top

FILE *f = fopen("a.txt", "r");
来源：http://llc.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vak.aibaodan.cn

fclose(f);
来源：http://anj.daxiang520.top

[S12] C：写文件
来源：http://gvd.52xcode.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mwh.smart0.xyz

[S13] C：宏定义
来源：http://fue.cucudq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lim.jinqigfzy.top

[S14] C：枚举
来源：http://lah.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://gdl.jqgfzy.top

[S15] C：类型转换
来源：http://yga.jianghu66.top

(double) a / b
来源：http://bra.jianghu66.top

[S16] C：位操作置位
来源：http://eze.hcnkem.com

x |= (1 << 3);
来源：http://nxf.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://aob.shanyushiyangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zxq.fengsongda.top

[S18] C：命令行参数
来源：http://aus.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://bvk.fanxiaobao.xyz

[S19] C：快速排序
来源：http://xiq.xinyue.icu

qsort(a, n, sizeof(int), cmp);
来源：http://jkv.pycfn.com

[S20] C：二分查找
来源：http://dyb.sysykeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://svf.sweek.top

[S21] C：字符类别判断
来源：http://exi.hammf.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uiz.ehwqpu.com

[S22] C：字符串转数字
来源：http://qks.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gpu.pengpengdd.cyou

[S23] C：随机数
来源：http://nlh.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://whq.xuanzx.com

[S24] C：获取本地时间
来源：http://ble.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sog.nanxinkj.top

[S25] C：内存拷贝
来源：http://zts.cucudq.cn

memcpy(dst, src, n);
来源：http://gmn.tanke756.top

[S26] C：内存清零
来源：http://hxd.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://xmg.zhaomingkeji.xyz

[S27] C：定义常量
来源：http://xtn.zhiwuduotai.top

const double PI = 3.14159;
来源：http://azy.aibaodan.cn

[S28] C：静态变量
来源：http://fcc.ivvv.top

static int counter = 0;
来源：http://mky.9152youxi.cn

[S29] C：变参函数
来源：http://lqc.yfazqb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rjm.cashguo.top

[S30] C：头文件保护
来源：http://gjx.yuanzhike.top

#ifndef X_H
来源：http://bjg.ppjwa.cn

#define X_H
来源：http://czy.ydzc1.top

#endif
来源：http://wbs.andypj.xyz

[S31] C++：Hello World
来源：http://gxu.hysaishi.cn

#include <iostream>
来源：http://aov.xinyue.icu

int main() { std::cout << "Hello\n"; }
来源：http://chh.zhongyouzk.top

[S32] C++：字符串
来源：http://zlk.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://ame.chenlongwang.top

[S33] C++：vector 增删
来源：http://dcg.birdmap.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aww.52xcode.cn

[S34] C++：遍历 vector
来源：http://apm.fengsongda.top

for (auto &x : v) { std::cout << x; }
来源：http://yjg.yuanzhike.top

[S35] C++：map
来源：http://cjx.fktsv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ekd.cucudq.cn

[S36] C++：unordered_map
来源：http://zov.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://frk.zhoulong.xyz

[S37] C++：set
来源：http://ydk.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tzv.ppjwa.cn

[S38] C++：排序
来源：http://kud.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://gki.gogol.net.cn

[S39] C++：自定义比较器排序
来源：http://sse.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://msf.gotoacloud.top

[S40] C++：查找元素
来源：http://puz.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eun.zhixingplan.top

[S41] C++：类与构造函数
来源：http://met.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ndj.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://fyr.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://fnu.hfpthk.cn

[S43] C++：智能指针
来源：http://hgw.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://bti.zycfv.cn

[S44] C++：引用传参
来源：http://qsw.cucudq.cn

void inc(int &x) { ++x; }
来源：http://pre.shanyushiyangtech.top

[S45] C++：lambda
来源：http://vvg.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://gba.daxiang520.top

[S46] C++：函数模板
来源：http://vcu.hfpthk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gos.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://hqt.hnxiangtu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ani.bjfxy.top

[S48] C++：逐行读文件
来源：http://mwf.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kui.sweek.top

while (std::getline(in, line)) { }
来源：http://ops.yongpay.top

[S49] C++：写文件
来源：http://ddx.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qah.gaohongyu789.top

[S50] C++：格式化数字
来源：http://ukf.pycfn.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nnp.c1oappe.top

[S51] C++：显式类型转换
来源：http://ybl.sysykeji.top

static_cast<double>(a) / b
来源：http://ctq.ctjpmb.com

[S52] C++：const 与 noexcept
来源：http://xpo.ctjpmb.com

int size() const noexcept { return n_; }
来源：http://koe.jlsjyb.cn

[S53] C++：移动语义
来源：http://hkb.hammf.cn

std::vector<int> w = std::move(v);
来源：http://gwc.dianchejie.cn

[S54] C++：异常处理
来源：http://okm.fktsv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tvv.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://ogf.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oda.cucudq.cn

[S56] C++：optional
来源：http://nss.sysykeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vxj.cdnleiting.top

[S57] C++：编译期常量
来源：http://tfn.bjfxy.top

constexpr int N = 10;
来源：http://hli.cheryme.top

[S58] C++：命名空间
来源：http://lwx.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://bcs.zhaomingkeji.xyz

[S59] C++：静态断言
来源：http://fvd.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lcj.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://rsb.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cqe.zdbjq.cn

================================================================================
来源：http://cjm.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mkf.yangfankeji.com

================================================================================
来源：http://lgf.aizwys.cn

[T01] Kotlin：Hello World
来源：http://cqe.snrcjt.cn

println("Hello")
来源：http://gyo.daxiang520.top

[T02] Kotlin：变量
来源：http://txy.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tdu.pycfn.com

[T03] Kotlin：字符串模板
来源：http://hkp.cheryme.top

"值: $b"
来源：http://oqu.zhixingplan.top

[T04] Kotlin：空安全
来源：http://yni.jinqigufen.top

val n: String? = null;  n?.length
来源：http://vpf.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://das.yangfankeji.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ixm.yuxming.cn

[T06] Kotlin：集合映射
来源：http://bfa.wangdashe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bgm.chenzaomai.com


<!-- 参考信息 -->