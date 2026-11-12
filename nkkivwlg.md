代发 wailian999

set -euo pipefail
来源：http://cvb.vehdjk.com

[R02] 变量赋值与使用
来源：http://rra.ctjpmb.com

name="Tom"; echo "$name"
来源：http://osp.cheryme.top

[R03] 只读变量
来源：http://ugh.mhx1999.top

readonly PI=3.14
来源：http://qfi.dashuyun.cn

[R04] 位置参数
来源：http://rre.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xuu.zhixingplan.top

[R05] 参数默认值
来源：http://ifw.fengsongda.top

name="${1:-default}"
来源：http://eqv.xylfe.cn

[R06] 判断命令是否存在
来源：http://uvg.vehdjk.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dql.yj20258888.top

[R07] if 判断文件
来源：http://jie.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ezt.dashuyun.cn

[R08] 数值比较
来源：http://ahv.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ymn.hnqzz.top

[R09] 字符串比较
来源：http://qvq.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://usr.tanke756.top

[R10] 正则匹配
来源：http://bca.aibaodan.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uhw.havefunace.top

[R11] case 多分支
来源：http://lkn.gogol.net.cn

case "$1" in
来源：http://wie.xziqi.cn

start) echo "启动" ;;
来源：http://cbh.gotoacloud.top

stop)  echo "停止" ;;
来源：http://rve.birdmap.top

*)     echo "未知命令" ;;
来源：http://uye.yuanzhike.top

esac
来源：http://brm.jqgufenzy.top

[R12] for 遍历文件
来源：http://uir.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://zhu.zdqjudy.top

[R13] for 计数循环
来源：http://frf.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://jtt.daxiang520.top

[R14] C 风格 for
来源：http://tmi.xuanzx.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jyk.yonumen.top

[R15] while 逐行读文件
来源：http://sfp.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ohx.nanxinkj.top

[R16] until 等待条件
来源：http://kih.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jhm.vehdjk.com

[R17] 数组定义与取值
来源：http://aup.zhixingplan.top

arr=(a b c); echo "${arr[0]}"
来源：http://sjt.zdqjudy.top

[R18] 遍历数组
来源：http://ubv.52xcode.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tzk.316326.xyz

[R19] 数组长度
来源：http://rej.tian-w.cn

echo "${#arr[@]}"
来源：http://ncl.pycfn.com

[R20] 关联数组（字典）
来源：http://kph.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nmn.bbcook.cn

[R21] 字符串长度
来源：http://czv.yj20258888.top

echo "${#s}"
来源：http://mfw.yonumen.top

[R22] 截取子串
来源：http://swo.nanxinkj.top

echo "${s:0:5}"
来源：http://ljo.epnwcf.com

[R23] 字符串替换
来源：http://nul.cdnleiting.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lok.yangfankeji.com

[R24] 大小写转换
来源：http://cqe.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://vhk.nwbrower.top

[R25] 去后缀 / 去前缀
来源：http://axg.yongpay.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fyk.hesvh.cn

[R26] 命令替换
来源：http://vjk.yongpay.top

now=$(date +%F); echo "$now"
来源：http://bdd.xziqi.cn

[R27] 算术展开
来源：http://dlk.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://lqx.bbcook.cn

[R28] 浮点运算
来源：http://nnh.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://efc.yanxiufei.cn

[R29] 定义函数
来源：http://nvy.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lzs.quarkkingdee.top

[R30] 函数返回状态码
来源：http://eof.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://eny.yonumen.top

[R31] 局部变量
来源：http://fme.hnqzz.top

f() { local x=1; echo "$x"; }
来源：http://eat.xylfe.cn

[R32] 参数个数校验
来源：http://gph.redwolf501.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://myl.sweek.top

[R33] 捕获错误并提示行号
来源：http://meh.shanyushiyangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ajf.meibo888.top

[R34] 退出时清理
来源：http://szy.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tjt.xuanzx.com

[R35] 后台执行并等待
来源：http://sou.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://enh.0kj1m.cn

[R36] 并发执行多个任务
来源：http://ftq.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mmg.sufxvd.cn

[R37] 把输出赋给变量
来源：http://skh.sysykeji.top

files=$(ls -1)
来源：http://lng.yuxming.cn

[R38] 管道串联
来源：http://xch.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://mut.dianchejie.cn

[R39] 重定向标准输出与错误
来源：http://rkh.epnwcf.com

cmd > out.log 2>&1
来源：http://mwl.redwolf501.top

[R40] 追加写日志
来源：http://qnj.shanyushiyangkeji.top

echo "log" >> out.log
来源：http://evj.smart0.xyz

[R41] 丢弃输出
来源：http://btg.gotoacloud.top

cmd >/dev/null 2>&1
来源：http://haf.fanxiaobao.xyz

[R42] 输入重定向
来源：http://ekc.tanke756.top

wc -l < a.txt
来源：http://zmq.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://tqq.svipenyu.cn

find . -name "*.log" -type f
来源：http://lqh.epnwcf.com

[R44] 按修改时间查找
来源：http://ysr.zhijiandao.cn

find . -mtime -7 -type f
来源：http://hgq.zdqjudy.top

[R45] 批量删除
来源：http://cxo.meibo888.top

find . -name "*.tmp" -delete
来源：http://pyy.sjlbkw.cn

[R46] 递归替换文件内容
来源：http://ftr.zhongyouzk.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tmy.bbcook.cn

[R47] sed 单行替换
来源：http://lyw.zhaomingkeji.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://cnb.nanxuanxn.top

[R48] awk 取指定列
来源：http://thw.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://ipx.tarul.cn

[R49] awk 带条件
来源：http://agv.c1oappe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ynx.gogol.net.cn

[R50] awk 求和
来源：http://vie.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://fzr.cucudq.cn

[R51] 排序去重取前几
来源：http://ilm.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://shj.hfpthk.cn

[R52] 统计行数
来源：http://bre.yvedp.cn

wc -l a.txt
来源：http://atv.ppjwa.cn

[R53] 查看文件头与实时尾
来源：http://ckp.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ljz.gogol.net.cn

[R54] 比较两个文件
来源：http://clt.tian-w.cn

diff a.txt b.txt
来源：http://zze.andypj.xyz

[R55] 压缩与解压
来源：http://qjc.zhengqikj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fqn.shanyushiyangtech.top

[R56] 远程拷贝
来源：http://hyj.iojbl.cn

scp file user@host:/path/
来源：http://arb.jinyuanbaomall.cn

[R57] 远程执行命令
来源：http://ixv.jiagoushi.top

ssh user@host 'uptime'
来源：http://yir.feifeiyinyue.top

[R58] 下载文件
来源：http://wzc.xylfe.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cjg.aizwys.cn

[R59] 发 POST JSON
来源：http://rua.andypj.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wcl.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://smi.yanxiufei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://knf.52xcode.cn

[R61] 磁盘占用
来源：http://jjf.jinqigfzy.top

df -h;  du -sh *
来源：http://jkm.jqgfzy.top

[R62] 找最占空间的文件
来源：http://eej.guannengcc.top

du -ah . | sort -rh | head -10
来源：http://zjy.yanxiufei.cn

[R63] 内存与进程
来源：http://tbj.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://kuw.jinyuanbaomall.cn

[R64] 结束进程
来源：http://fyb.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://vyz.wangdashe.top

[R65] 查看端口占用
来源：http://xmu.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uop.sweek.top

[R66] 定时任务
来源：http://jam.nwbrower.top

crontab -e;  crontab -l
来源：http://tmu.jinghuilouyu.cn

[R67] 生成随机十六进制串
来源：http://iwv.bbcook.cn

openssl rand -hex 16
来源：http://zfh.zhaomingkeji.xyz

[R68] 计算文件校验值
来源：http://juc.hesvh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://eav.hammf.cn

[R69] 生成随机密码
来源：http://vti.zhongyouzk.top

head -c 16 /dev/urandom | base64
来源：http://znk.316326.xyz

[R70] 时间戳与互转
来源：http://qyl.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://mtr.sxryk.cn

[R71] 日期格式化
来源：http://pzz.nwbrower.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://oga.yj20258.top

[R72] 等待端口就绪
来源：http://icv.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hed.hammf.cn

[R73] 分割大日志
来源：http://epz.bjfxy.top

split -l 1000 big.log part_
来源：http://cyj.hnxiangtu.top

[R74] 批量重命名
来源：http://jqh.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://olq.vehdjk.com

[R75] 导出环境变量
来源：http://fph.zhixingplan.top

export PATH="$HOME/bin:$PATH"
来源：http://sxa.dianchejie.cn

[R76] 使用临时文件
来源：http://ucc.feifeiyinyue.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ipq.wangshuangyany.cn

[R77] 读取用户输入
来源：http://aeh.tarul.cn

read -rp "请输入: " ans
来源：http://kaj.zhaomingkeji.xyz

[R78] 交互式菜单
来源：http://hev.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bub.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://oas.chenzaomai.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uyl.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://hll.xylfe.cn

time ./run.sh
来源：http://ytu.cheryme.top

================================================================================
来源：http://ovg.wangdashe.top

S. C / C++ 专题
来源：http://vox.hongshengwenyu.top

================================================================================
来源：http://jph.cashguo.top

[S01] C：Hello World
来源：http://tnj.cheryme.top

#include <stdio.h>
来源：http://wbk.shangyingyoupin.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rdo.kuanghao11.cn

[S02] C：变量与格式化输出
来源：http://oxc.ybcxt.top

int a = 10; printf("%d\n", a);
来源：http://lmx.yueranfly.top

[S03] C：读入整数
来源：http://wyp.haohaochexian.top

int x; scanf("%d", &x);
来源：http://lfb.vqdsnc.cn

[S04] C：字符串复制
来源：http://lez.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://zzf.jqgufenzy.top

[S05] C：字符串长度
来源：http://cay.nanxinkj.top

strlen(s)
来源：http://pih.jinghuilouyu.cn

[S06] C：字符串比较
来源：http://zrb.jiagoushi.top

strcmp(a, b) == 0
来源：http://nxk.bjfxy.top

[S07] C：数组遍历求和
来源：http://hxn.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dnr.hcnkem.com

[S08] C：动态内存分配与释放
来源：http://jnc.bjfxy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eli.jlsjyb.cn

[S09] C：结构体定义与初始化
来源：http://zdc.svipenyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lbk.ctjpmb.com

[S10] C：指针与解引用
来源：http://ogs.zhengqikj.top

int *p = &a;  *p = 5;
来源：http://bhz.52xcode.cn

[S11] C：逐行读文件
来源：http://lgh.shuidangran.top

FILE *f = fopen("a.txt", "r");
来源：http://fwt.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xyo.aizwys.cn

fclose(f);
来源：http://jrw.xylfe.cn

[S12] C：写文件
来源：http://yaz.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rfj.bjfxy.top

[S13] C：宏定义
来源：http://kuw.yj20258.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kfv.hfpthk.cn

[S14] C：枚举
来源：http://dfc.guowangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://mdh.cheryme.top

[S15] C：类型转换
来源：http://wdp.pycfn.com

(double) a / b
来源：http://phw.yuanzhike.top

[S16] C：位操作置位
来源：http://csz.nanxinkj.top

x |= (1 << 3);
来源：http://cxp.fzhhl.top

[S17] C：安全拼接字符串
来源：http://umz.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://slt.jqgufenzy.top

[S18] C：命令行参数
来源：http://jwt.fehbvm.com

int main(int argc, char **argv)
来源：http://yen.nanxinkj.top

[S19] C：快速排序
来源：http://uce.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://igt.nanxinkj.top

[S20] C：二分查找
来源：http://rta.svipenyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bic.zhongyouzk.top

[S21] C：字符类别判断
来源：http://sjo.pycfn.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://osy.zdqjudy.top

[S22] C：字符串转数字
来源：http://bep.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ubj.tarul.cn

[S23] C：随机数
来源：http://hcz.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yis.chenzaomai.com

[S24] C：获取本地时间
来源：http://btc.yangfankeji.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hgr.aibaodan.cn

[S25] C：内存拷贝
来源：http://hay.sysykeji.top

memcpy(dst, src, n);
来源：http://rmw.shzxlz.cn

[S26] C：内存清零
来源：http://hhi.yfazqb.com

memset(a, 0, sizeof a);
来源：http://icm.tianlin.xyz

[S27] C：定义常量
来源：http://yyw.kuanghao11.cn

const double PI = 3.14159;
来源：http://gse.gzhubu.top

[S28] C：静态变量
来源：http://ald.hnqzz.top

static int counter = 0;
来源：http://llx.ctjpmb.com

[S29] C：变参函数
来源：http://ckb.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cna.ehwqpu.com

[S30] C：头文件保护
来源：http://rdo.ybcxt.top

#ifndef X_H
来源：http://lht.shuidangran.top

#define X_H
来源：http://xeg.tanke756.top

#endif
来源：http://qlc.ywan-chungtsiang.top

[S31] C++：Hello World
来源：http://igx.xylfe.cn

#include <iostream>
来源：http://kxf.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://dtb.fehbvm.com

[S32] C++：字符串
来源：http://jdk.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://wmx.jinyuanbaomall.cn

[S33] C++：vector 增删
来源：http://kca.zhijiandao.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xta.jinqigufen.top

[S34] C++：遍历 vector
来源：http://heo.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://ksv.dianchejie.cn

[S35] C++：map
来源：http://imv.daria6918.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://klp.nanxinkj.top

[S36] C++：unordered_map
来源：http://vuj.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ker.zdbjq.cn

[S37] C++：set
来源：http://pfb.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xjv.ehwqpu.com

[S38] C++：排序
来源：http://fcl.fehbvm.com

std::sort(v.begin(), v.end());
来源：http://cok.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://eny.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wym.sweek.top

[S40] C++：查找元素
来源：http://qmy.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wjj.iojbl.cn

[S41] C++：类与构造函数
来源：http://rlj.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://glq.hesvh.cn

[S42] C++：继承与虚函数
来源：http://nxy.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://pzy.zycfv.cn

[S43] C++：智能指针
来源：http://ylv.9152youxi.cn

auto p = std::make_unique<int>(5);
来源：http://rzi.xylfe.cn

[S44] C++：引用传参
来源：http://bex.mhx1999.top

void inc(int &x) { ++x; }
来源：http://xdb.nanxinkj.top

[S45] C++：lambda
来源：http://xdv.vqdsnc.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xnp.9152youxi.cn

[S46] C++：函数模板
来源：http://box.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tkd.ivvv.top

[S47] C++：结构化绑定遍历
来源：http://ycm.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qdl.nwbrower.top

[S48] C++：逐行读文件
来源：http://thz.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uxb.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://jbu.fzhhl.top

[S49] C++：写文件
来源：http://ttg.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mol.gogol.net.cn

[S50] C++：格式化数字
来源：http://hse.tian-w.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vrl.smart0.xyz

[S51] C++：显式类型转换
来源：http://ewu.jinqigufen.top

static_cast<double>(a) / b
来源：http://uoz.bjfxy.top

[S52] C++：const 与 noexcept
来源：http://vms.chenzaomai.com

int size() const noexcept { return n_; }
来源：http://rbt.52xcode.cn

[S53] C++：移动语义
来源：http://pfh.fktsv.cn

std::vector<int> w = std::move(v);
来源：http://klq.iojbl.cn

[S54] C++：异常处理
来源：http://qzr.yj20258888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lur.jlsjyb.cn

[S55] C++：结构化绑定
来源：http://inf.gotoacloud.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ark.gogol.net.cn

[S56] C++：optional
来源：http://fsr.hcnkem.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wvz.aibaodan.cn

[S57] C++：编译期常量
来源：http://syj.ctjpmb.com

constexpr int N = 10;
来源：http://exg.fzhhl.top

[S58] C++：命名空间
来源：http://esw.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://izf.sjlbkw.cn

[S59] C++：静态断言
来源：http://jjz.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xku.vehdjk.com

[S60] C++：遍历并删除元素
来源：http://tsp.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aiw.ybcxt.top

================================================================================
来源：http://fnj.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gzy.ydjk.org.cn

================================================================================
来源：http://rtd.zhaomingkeji.xyz

[T01] Kotlin：Hello World
来源：http://hpi.dashuyun.cn

println("Hello")
来源：http://vdp.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://qkr.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pot.xuetiantiany.cn


<!-- 参考信息 -->