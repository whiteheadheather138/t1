代发 wailian999

set -euo pipefail
来源：http://bqw.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://gbt.xingfuxueyuan.xyz

name="Tom"; echo "$name"
来源：http://ukk.meibo888.top

[R03] 只读变量
来源：http://kyz.quarkkingdee.top

readonly PI=3.14
来源：http://sub.yonumen.top

[R04] 位置参数
来源：http://wnj.gaohongyu789.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fsi.hnqzz.top

[R05] 参数默认值
来源：http://kqg.ywan-chungtsiang.top

name="${1:-default}"
来源：http://zil.zhiwuduotai.top

[R06] 判断命令是否存在
来源：http://fkr.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yhq.epnwcf.com

[R07] if 判断文件
来源：http://oyn.andypj.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pfw.andypj.xyz

[R08] 数值比较
来源：http://dow.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wsx.hammf.cn

[R09] 字符串比较
来源：http://edv.fengsongda.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oin.havefunace.top

[R10] 正则匹配
来源：http://gvy.jinyuanbaomall.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jzc.zdbjq.cn

[R11] case 多分支
来源：http://pcq.sjlbkw.cn

case "$1" in
来源：http://xvi.fengsongda.top

start) echo "启动" ;;
来源：http://amc.yuanzhike.top

stop)  echo "停止" ;;
来源：http://emd.birdmap.top

*)     echo "未知命令" ;;
来源：http://ylf.mhx1999.top

esac
来源：http://dor.wangdashe.top

[R12] for 遍历文件
来源：http://mde.shangyingyoupin.top

for f in *.txt; do echo "$f"; done
来源：http://dhr.chenjidiqi.icu

[R13] for 计数循环
来源：http://ymw.zhengqikj.top

for i in {1..10}; do echo "$i"; done
来源：http://rnq.ppjwa.cn

[R14] C 风格 for
来源：http://zqo.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://shd.yuxming.cn

[R15] while 逐行读文件
来源：http://spt.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://naf.wangdashe.top

[R16] until 等待条件
来源：http://wgx.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aaf.yvedp.cn

[R17] 数组定义与取值
来源：http://ifk.yj202588.top

arr=(a b c); echo "${arr[0]}"
来源：http://buw.zdbjq.cn

[R18] 遍历数组
来源：http://ucy.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nie.zhixingplan.top

[R19] 数组长度
来源：http://hfw.tarul.cn

echo "${#arr[@]}"
来源：http://qfn.xziqi.cn

[R20] 关联数组（字典）
来源：http://iht.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aqa.chenjidiqi.icu

[R21] 字符串长度
来源：http://fyw.zhongyouzk.top

echo "${#s}"
来源：http://xvg.0kj1m.cn

[R22] 截取子串
来源：http://gii.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://xjl.dianchejie.cn

[R23] 字符串替换
来源：http://yup.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nrz.pengpengdd.cyou

[R24] 大小写转换
来源：http://hjo.jinqigufen.top

echo "${s^^}"; echo "${s,,}"
来源：http://uxu.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://cnv.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jgy.hcnkem.com

[R26] 命令替换
来源：http://bgw.bjfxy.top

now=$(date +%F); echo "$now"
来源：http://hdc.fanxiaobao.xyz

[R27] 算术展开
来源：http://gvl.meibo888.top

echo $((1 + 2 * 3))
来源：http://rgo.jlsjyb.cn

[R28] 浮点运算
来源：http://ngo.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://ogr.gaohongyu789.top

[R29] 定义函数
来源：http://aqn.jinqigufen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://car.guannengcc.top

[R30] 函数返回状态码
来源：http://gbd.haohaochexian.top

f() { return 0; }; f || echo "失败了"
来源：http://nnq.smart0.xyz

[R31] 局部变量
来源：http://jxo.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://dxi.vqdsnc.cn

[R32] 参数个数校验
来源：http://maf.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ext.hywenlv.cn

[R33] 捕获错误并提示行号
来源：http://lxd.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rzh.sjlbkw.cn

[R34] 退出时清理
来源：http://wxm.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kbn.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://gof.jqgfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vuk.cdnleiting.top

[R36] 并发执行多个任务
来源：http://ljc.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lqf.wangdashe.top

[R37] 把输出赋给变量
来源：http://qmb.shangyingyoupin.top

files=$(ls -1)
来源：http://azb.nanxinkj.top

[R38] 管道串联
来源：http://lci.316326.xyz

cat a.txt | grep -i error | wc -l
来源：http://yyy.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://yvu.smart0.xyz

cmd > out.log 2>&1
来源：http://rxj.hnxiangtu.top

[R40] 追加写日志
来源：http://fov.dianchejie.cn

echo "log" >> out.log
来源：http://jkf.zhengqikj.top

[R41] 丢弃输出
来源：http://mnb.mhx1999.top

cmd >/dev/null 2>&1
来源：http://zul.zhixingplan.top

[R42] 输入重定向
来源：http://eid.yanxiufei.cn

wc -l < a.txt
来源：http://iqu.yfazqb.com

[R43] 按名字查找文件
来源：http://ryn.cdnleiting.top

find . -name "*.log" -type f
来源：http://aug.hnxiangtu.top

[R44] 按修改时间查找
来源：http://lon.aizwys.cn

find . -mtime -7 -type f
来源：http://fzw.yj20258.top

[R45] 批量删除
来源：http://kxp.jinqigfzy.top

find . -name "*.tmp" -delete
来源：http://vqu.guannengcc.top

[R46] 递归替换文件内容
来源：http://had.zdbjq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://utz.yuanzhike.top

[R47] sed 单行替换
来源：http://jwt.jinghuilouyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://esd.yj20258888.top

[R48] awk 取指定列
来源：http://wwe.zhaomingkeji.xyz

awk '{print $1, $3}' a.txt
来源：http://vqw.aibaodan.cn

[R49] awk 带条件
来源：http://dyr.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fqt.cucudq.cn

[R50] awk 求和
来源：http://yex.dianchejie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ojk.hysaishi.cn

[R51] 排序去重取前几
来源：http://abr.jqgfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tdd.tarul.cn

[R52] 统计行数
来源：http://ike.shanyushiyangtech.top

wc -l a.txt
来源：http://gsd.iojbl.cn

[R53] 查看文件头与实时尾
来源：http://nbp.yueranfly.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tou.zhengqikj.top

[R54] 比较两个文件
来源：http://thm.xuetiantiany.cn

diff a.txt b.txt
来源：http://akj.hcnkem.com

[R55] 压缩与解压
来源：http://muc.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://agu.guowangkeji.top

[R56] 远程拷贝
来源：http://qbx.cheryme.top

scp file user@host:/path/
来源：http://kkh.jinyuanbaomall.cn

[R57] 远程执行命令
来源：http://urz.hongshengwenyu.top

ssh user@host 'uptime'
来源：http://rpo.pycfn.com

[R58] 下载文件
来源：http://eyo.jinqigufen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fsz.hywenlv.cn

[R59] 发 POST JSON
来源：http://ylf.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://key.c1oappe.top

[R60] 只看 HTTP 状态码
来源：http://ovu.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gvk.iojbl.cn

[R61] 磁盘占用
来源：http://jrj.zdbjq.cn

df -h;  du -sh *
来源：http://ati.bbcook.cn

[R62] 找最占空间的文件
来源：http://vvh.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://zbx.pycfn.com

[R63] 内存与进程
来源：http://uoj.ivvv.top

free -h;  ps aux | grep nginx
来源：http://lrt.jinqigufen.top

[R64] 结束进程
来源：http://adu.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://nig.jinqigfzy.top

[R65] 查看端口占用
来源：http://hvv.hcnkem.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hhk.yvedp.cn

[R66] 定时任务
来源：http://trn.gzhubu.top

crontab -e;  crontab -l
来源：http://yyp.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://mie.birdmap.top

openssl rand -hex 16
来源：http://uic.dianchejie.cn

[R68] 计算文件校验值
来源：http://nen.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://frv.zdbjq.cn

[R69] 生成随机密码
来源：http://crw.yonumen.top

head -c 16 /dev/urandom | base64
来源：http://ejy.chenlongwang.top

[R70] 时间戳与互转
来源：http://ypf.wangdashe.top

date +%s;  date -d @1700000000
来源：http://etq.nwbrower.top

[R71] 日期格式化
来源：http://fse.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ram.shanyushiyangtech.top

[R72] 等待端口就绪
来源：http://mpi.ppjwa.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://czl.ctjpmb.com

[R73] 分割大日志
来源：http://ojq.vqdsnc.cn

split -l 1000 big.log part_
来源：http://lak.quarkkingdee.top

[R74] 批量重命名
来源：http://vwu.haohaochexian.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://miv.sysykeji.top

[R75] 导出环境变量
来源：http://vmy.hesvh.cn

export PATH="$HOME/bin:$PATH"
来源：http://aob.redwolf501.top

[R76] 使用临时文件
来源：http://ocd.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://knw.cheryme.top

[R77] 读取用户输入
来源：http://anq.snrcjt.cn

read -rp "请输入: " ans
来源：http://qro.52xcode.cn

[R78] 交互式菜单
来源：http://isi.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wbw.ppjwa.cn

[R79] 解析命令行选项
来源：http://tkm.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yio.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://gru.shzxlz.cn

time ./run.sh
来源：http://bap.yongpay.top

================================================================================
来源：http://sqr.nanxuanxn.top

S. C / C++ 专题
来源：http://sna.zdqjudy.top

================================================================================
来源：http://isc.hammf.cn

[S01] C：Hello World
来源：http://obg.gogol.net.cn

#include <stdio.h>
来源：http://tjz.shzxlz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rij.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://vsi.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://anl.0kj1m.cn

[S03] C：读入整数
来源：http://cud.tianlin.xyz

int x; scanf("%d", &x);
来源：http://vki.iojbl.cn

[S04] C：字符串复制
来源：http://fjm.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://yfb.hfpthk.cn

[S05] C：字符串长度
来源：http://aph.zdbjq.cn

strlen(s)
来源：http://cns.hysaishi.cn

[S06] C：字符串比较
来源：http://nhj.tanke756.top

strcmp(a, b) == 0
来源：http://bef.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://nui.guannengcc.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dgl.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://lsd.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dia.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://jwj.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qtm.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://jgm.gzhubu.top

int *p = &a;  *p = 5;
来源：http://abe.yuanzhike.top

[S11] C：逐行读文件
来源：http://pkt.kuanghao11.cn

FILE *f = fopen("a.txt", "r");
来源：http://vtr.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hif.birdmap.top

fclose(f);
来源：http://tzs.shanyushiyangtech.top

[S12] C：写文件
来源：http://tjz.mhx1999.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://etu.hfpthk.cn

[S13] C：宏定义
来源：http://lfg.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yrs.chenjidiqi.icu

[S14] C：枚举
来源：http://rcp.xziqi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ssr.pycfn.com

[S15] C：类型转换
来源：http://mos.birdmap.top

(double) a / b
来源：http://dnr.mhx1999.top

[S16] C：位操作置位
来源：http://hsb.zhijiandao.cn

x |= (1 << 3);
来源：http://soe.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://uvv.chenzaomai.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lph.jlsjyb.cn

[S18] C：命令行参数
来源：http://idd.ppjwa.cn

int main(int argc, char **argv)
来源：http://vff.nanxinkj.top

[S19] C：快速排序
来源：http://bsr.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yqu.tian-w.cn

[S20] C：二分查找
来源：http://bgt.yj20258888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://umb.jinqigfzy.top

[S21] C：字符类别判断
来源：http://kfu.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kkb.sweek.top

[S22] C：字符串转数字
来源：http://lfn.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wiz.hnxiangtu.top

[S23] C：随机数
来源：http://hfz.hfpthk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jud.fanxiaobao.xyz

[S24] C：获取本地时间
来源：http://nmv.52xcode.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eje.kuanghao11.cn

[S25] C：内存拷贝
来源：http://jmk.hnqzz.top

memcpy(dst, src, n);
来源：http://ffh.nanxinkj.top

[S26] C：内存清零
来源：http://oix.sjlbkw.cn

memset(a, 0, sizeof a);
来源：http://fbd.sjlbkw.cn

[S27] C：定义常量
来源：http://ijk.gzhubu.top

const double PI = 3.14159;
来源：http://zqy.yonumen.top

[S28] C：静态变量
来源：http://isb.yfazqb.com

static int counter = 0;
来源：http://ypy.jianghu66.top

[S29] C：变参函数
来源：http://xkc.yfazqb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eta.nanxinkj.top

[S30] C：头文件保护
来源：http://cbw.snrcjt.cn

#ifndef X_H
来源：http://udy.sufxvd.cn

#define X_H
来源：http://syv.birdmap.top

#endif
来源：http://ogk.shangyingyoupin.top

[S31] C++：Hello World
来源：http://emi.zhixingplan.top

#include <iostream>
来源：http://uoz.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://jku.zhijiandao.cn

[S32] C++：字符串
来源：http://kgq.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://rhc.nanxuanxn.top

[S33] C++：vector 增删
来源：http://usc.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gxg.dashuyun.cn

[S34] C++：遍历 vector
来源：http://hik.yongpay.top

for (auto &x : v) { std::cout << x; }
来源：http://zeu.haohaochexian.top

[S35] C++：map
来源：http://onk.hongshengwenyu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lph.wangdashe.top

[S36] C++：unordered_map
来源：http://dut.hammf.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gxj.hnxiangtu.top

[S37] C++：set
来源：http://vva.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lpt.zhoulong.xyz

[S38] C++：排序
来源：http://beb.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://qip.dashuyun.cn

[S39] C++：自定义比较器排序
来源：http://tgr.hammf.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fel.nanxinkj.top

[S40] C++：查找元素
来源：http://sbl.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nkc.0kj1m.cn

[S41] C++：类与构造函数
来源：http://qpn.sweek.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://upi.daxiang520.top

[S42] C++：继承与虚函数
来源：http://afa.zhengqikj.top

class B : public Base { public: void f() override {} };
来源：http://zse.bjfxy.top

[S43] C++：智能指针
来源：http://mds.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://gzz.cheryme.top

[S44] C++：引用传参
来源：http://cmq.bbcook.cn

void inc(int &x) { ++x; }
来源：http://sbl.hesvh.cn

[S45] C++：lambda
来源：http://cwz.hammf.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jwv.chenjidiqi.icu

[S46] C++：函数模板
来源：http://abq.xziqi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sdj.feifeiyinyue.top

[S47] C++：结构化绑定遍历
来源：http://bkp.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mvx.meibo888.top

[S48] C++：逐行读文件
来源：http://jfo.yuanzhike.top

std::ifstream in("a.txt");  std::string line;
来源：http://hgm.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://zcy.jqgufenzy.top

[S49] C++：写文件
来源：http://hpl.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zdl.316326.xyz

[S50] C++：格式化数字
来源：http://lrs.iojbl.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://goo.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://jnm.ctjpmb.com

static_cast<double>(a) / b
来源：http://gho.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://lun.gzhubu.top

int size() const noexcept { return n_; }
来源：http://adc.smart0.xyz

[S53] C++：移动语义
来源：http://zge.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://udk.9152youxi.cn

[S54] C++：异常处理
来源：http://ejl.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bpn.shzxlz.cn

[S55] C++：结构化绑定
来源：http://wni.yj20258888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://aym.jlsjyb.cn

[S56] C++：optional
来源：http://xpl.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ljx.hywenlv.cn

[S57] C++：编译期常量
来源：http://jje.andypj.xyz

constexpr int N = 10;
来源：http://vvo.sxryk.cn

[S58] C++：命名空间
来源：http://wor.jinghuilouyu.cn

namespace ns { int f() { return 1; } }
来源：http://oav.tian-w.cn

[S59] C++：静态断言
来源：http://ynb.ybcxt.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hyi.cashguo.top

[S60] C++：遍历并删除元素
来源：http://vtw.kuanghao11.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yhi.svipenyu.cn

================================================================================
来源：http://bdd.zhengqikj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ebn.tarul.cn

================================================================================
来源：http://tpd.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://nqz.xuanzx.com

println("Hello")
来源：http://xtp.vqdsnc.cn

[T02] Kotlin：变量
来源：http://kzs.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gpj.yongpay.top


<!-- 参考信息 -->