代发 wailian999

readonly PI=3.14
来源：http://nhj.tianlin.xyz

[R04] 位置参数
来源：http://dbu.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ajf.zhoulong.xyz

[R05] 参数默认值
来源：http://zkc.uphjek.com

name="${1:-default}"
来源：http://yii.0kj1m.cn

[R06] 判断命令是否存在
来源：http://eex.fehbvm.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fvd.nanxinkj.top

[R07] if 判断文件
来源：http://yud.aibaodan.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iin.zhixingplan.top

[R08] 数值比较
来源：http://jft.smart0.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://igz.wangdashe.top

[R09] 字符串比较
来源：http://jwt.zdbjq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mjl.fehbvm.com

[R10] 正则匹配
来源：http://epk.aibaodan.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wpc.sxryk.cn

[R11] case 多分支
来源：http://fge.yuxming.cn

case "$1" in
来源：http://hbd.jyoumei.cn

start) echo "启动" ;;
来源：http://fwn.zdqjudy.top

stop)  echo "停止" ;;
来源：http://peh.yvedp.cn

*)     echo "未知命令" ;;
来源：http://jgd.gotoacloud.top

esac
来源：http://vms.jqgfzy.top

[R12] for 遍历文件
来源：http://qri.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://cbp.redwolf501.top

[R13] for 计数循环
来源：http://yuw.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://hzw.daxiang520.top

[R14] C 风格 for
来源：http://vdo.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ykw.jyoumei.cn

[R15] while 逐行读文件
来源：http://kvi.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lsw.hcnkem.com

[R16] until 等待条件
来源：http://nuy.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cxh.yj202588.top

[R17] 数组定义与取值
来源：http://vri.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://fdd.uphjek.com

[R18] 遍历数组
来源：http://eix.cashguo.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rnq.yfazqb.com

[R19] 数组长度
来源：http://vlk.aibaodan.cn

echo "${#arr[@]}"
来源：http://ged.andypj.xyz

[R20] 关联数组（字典）
来源：http://ygv.gzhubu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fxr.cqqwz.cn

[R21] 字符串长度
来源：http://tjw.sufxvd.cn

echo "${#s}"
来源：http://sxx.zhixingplan.top

[R22] 截取子串
来源：http://roz.bjfxy.top

echo "${s:0:5}"
来源：http://rsw.jqgfzy.top

[R23] 字符串替换
来源：http://gno.zhoulong.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gxn.wangdashe.top

[R24] 大小写转换
来源：http://nxu.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://bfi.nwbrower.top

[R25] 去后缀 / 去前缀
来源：http://ini.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yyz.ydjk.org.cn

[R26] 命令替换
来源：http://fcg.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://zlm.zhongyouzk.top

[R27] 算术展开
来源：http://ekm.daxiang520.top

echo $((1 + 2 * 3))
来源：http://naz.zhiwuduotai.top

[R28] 浮点运算
来源：http://jti.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://wdq.hongshengwenyu.top

[R29] 定义函数
来源：http://wsw.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kpu.bjfxy.top

[R30] 函数返回状态码
来源：http://kap.ydjk.org.cn

f() { return 0; }; f || echo "失败了"
来源：http://atv.shanyushiyangkeji.top

[R31] 局部变量
来源：http://ggz.jiagoushi.top

f() { local x=1; echo "$x"; }
来源：http://ixv.gotoacloud.top

[R32] 参数个数校验
来源：http://bby.cheryme.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kpe.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://jzf.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://elz.aizwys.cn

[R34] 退出时清理
来源：http://lid.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xsn.hfpthk.cn

[R35] 后台执行并等待
来源：http://ulv.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://opt.birdmap.top

[R36] 并发执行多个任务
来源：http://lfc.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yqh.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://vjv.zdbjq.cn

files=$(ls -1)
来源：http://ine.yvedp.cn

[R38] 管道串联
来源：http://kjr.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://gdk.gotoacloud.top

[R39] 重定向标准输出与错误
来源：http://vpx.zhijiandao.cn

cmd > out.log 2>&1
来源：http://bit.sysykeji.top

[R40] 追加写日志
来源：http://pcg.cashguo.top

echo "log" >> out.log
来源：http://mlg.havefunace.top

[R41] 丢弃输出
来源：http://itm.uphjek.com

cmd >/dev/null 2>&1
来源：http://xpr.ctjpmb.com

[R42] 输入重定向
来源：http://ejn.52xcode.cn

wc -l < a.txt
来源：http://gqe.xingfuxueyuan.xyz

[R43] 按名字查找文件
来源：http://ncp.iojbl.cn

find . -name "*.log" -type f
来源：http://eht.sweek.top

[R44] 按修改时间查找
来源：http://gkw.epnwcf.com

find . -mtime -7 -type f
来源：http://lxg.yj202588.top

[R45] 批量删除
来源：http://ffz.ywan-chungtsiang.top

find . -name "*.tmp" -delete
来源：http://cse.xuanzx.com

[R46] 递归替换文件内容
来源：http://bmm.jianghu66.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nkh.hywenlv.cn

[R47] sed 单行替换
来源：http://zmi.zdbjq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ucg.yj20258888.top

[R48] awk 取指定列
来源：http://nfv.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://pqu.bbcook.cn

[R49] awk 带条件
来源：http://qct.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nll.shzxlz.cn

[R50] awk 求和
来源：http://zpk.cucudq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://alo.xuanzx.com

[R51] 排序去重取前几
来源：http://hin.hammf.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bml.zdqjudy.top

[R52] 统计行数
来源：http://gwc.jianghu66.top

wc -l a.txt
来源：http://xlb.jqgufenzy.top

[R53] 查看文件头与实时尾
来源：http://dci.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://naa.zhixingplan.top

[R54] 比较两个文件
来源：http://uod.iojbl.cn

diff a.txt b.txt
来源：http://pvm.zhengqikj.top

[R55] 压缩与解压
来源：http://kaq.chenjidiqi.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pxz.jinqigufen.top

[R56] 远程拷贝
来源：http://nfk.hnxiangtu.top

scp file user@host:/path/
来源：http://daf.hammf.cn

[R57] 远程执行命令
来源：http://jhp.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://oek.xziqi.cn

[R58] 下载文件
来源：http://xih.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qco.ctjpmb.com

[R59] 发 POST JSON
来源：http://cpj.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vvg.jqgufenzy.top

[R60] 只看 HTTP 状态码
来源：http://ibm.nanxinkj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yhq.ydzc1.top

[R61] 磁盘占用
来源：http://yzf.yueranfly.top

df -h;  du -sh *
来源：http://yam.wangdashe.top

[R62] 找最占空间的文件
来源：http://egz.sysykeji.top

du -ah . | sort -rh | head -10
来源：http://mzj.chenlongwang.top

[R63] 内存与进程
来源：http://ddc.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://ncv.hnqzz.top

[R64] 结束进程
来源：http://hls.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://gwa.9152youxi.cn

[R65] 查看端口占用
来源：http://xrz.shangyingyoupin.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://typ.ehwqpu.com

[R66] 定时任务
来源：http://buq.jinqigufen.top

crontab -e;  crontab -l
来源：http://ila.daxiang520.top

[R67] 生成随机十六进制串
来源：http://mut.yuanzhike.top

openssl rand -hex 16
来源：http://hvx.52xcode.cn

[R68] 计算文件校验值
来源：http://osh.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zix.vqdsnc.cn

[R69] 生成随机密码
来源：http://jnq.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://sct.mhx1999.top

[R70] 时间戳与互转
来源：http://gpi.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://oga.xylfe.cn

[R71] 日期格式化
来源：http://zrb.wangshuangyany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mfc.jqgfzy.top

[R72] 等待端口就绪
来源：http://hdz.jqgufenzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://atc.snrcjt.cn

[R73] 分割大日志
来源：http://stb.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://yeg.sufxvd.cn

[R74] 批量重命名
来源：http://tav.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kuh.tanke756.top

[R75] 导出环境变量
来源：http://gbn.nwbrower.top

export PATH="$HOME/bin:$PATH"
来源：http://daq.tanke756.top

[R76] 使用临时文件
来源：http://gwn.uphjek.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://urs.zhongyouzk.top

[R77] 读取用户输入
来源：http://zjy.cqqwz.cn

read -rp "请输入: " ans
来源：http://rhj.tianlin.xyz

[R78] 交互式菜单
来源：http://paj.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ejm.haohaochexian.top

[R79] 解析命令行选项
来源：http://pnr.zhaomingkeji.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dii.xuanzx.com

[R80] 查看脚本执行耗时
来源：http://htv.guowangkeji.top

time ./run.sh
来源：http://uqn.chenlongwang.top

================================================================================
来源：http://agm.zdqjudy.top

S. C / C++ 专题
来源：http://ncr.xingfuxueyuan.xyz

================================================================================
来源：http://pin.sxryk.cn

[S01] C：Hello World
来源：http://oct.yj20258.top

#include <stdio.h>
来源：http://jiu.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jgt.hammf.cn

[S02] C：变量与格式化输出
来源：http://pvn.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://ffy.shuidangran.top

[S03] C：读入整数
来源：http://ams.316326.xyz

int x; scanf("%d", &x);
来源：http://nkw.sxryk.cn

[S04] C：字符串复制
来源：http://prw.epnwcf.com

char dst[32]; strcpy(dst, "hi");
来源：http://afu.sysykeji.top

[S05] C：字符串长度
来源：http://bkr.fanxiaobao.xyz

strlen(s)
来源：http://xjk.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://eoy.chenlongwang.top

strcmp(a, b) == 0
来源：http://xcs.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://tct.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mul.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://env.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lle.birdmap.top

[S09] C：结构体定义与初始化
来源：http://wpm.jqgufenzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kkw.redwolf501.top

[S10] C：指针与解引用
来源：http://msj.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://zlf.c1oappe.top

[S11] C：逐行读文件
来源：http://czk.gzhubu.top

FILE *f = fopen("a.txt", "r");
来源：http://jmq.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hgv.yanxiufei.cn

fclose(f);
来源：http://mft.meibo888.top

[S12] C：写文件
来源：http://xiy.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mne.ivvv.top

[S13] C：宏定义
来源：http://mel.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zll.gogol.net.cn

[S14] C：枚举
来源：http://jil.yvedp.cn

enum Color { RED, GREEN, BLUE };
来源：http://fom.sufxvd.cn

[S15] C：类型转换
来源：http://stv.uphjek.com

(double) a / b
来源：http://dwx.sweek.top

[S16] C：位操作置位
来源：http://cgn.52xcode.cn

x |= (1 << 3);
来源：http://jkb.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://ghr.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lfl.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://bdc.kuanghao11.cn

int main(int argc, char **argv)
来源：http://mnc.hammf.cn

[S19] C：快速排序
来源：http://zvd.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://psq.tarul.cn

[S20] C：二分查找
来源：http://zdd.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ztq.bbcook.cn

[S21] C：字符类别判断
来源：http://yhw.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gad.epnwcf.com

[S22] C：字符串转数字
来源：http://mdz.zhongyouzk.top

atoi("42");  strtod("3.14", NULL);
来源：http://daz.gotoacloud.top

[S23] C：随机数
来源：http://bbj.yonumen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lil.dianchejie.cn

[S24] C：获取本地时间
来源：http://ynx.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dcq.guannengcc.top

[S25] C：内存拷贝
来源：http://nhx.smart0.xyz

memcpy(dst, src, n);
来源：http://gys.0kj1m.cn

[S26] C：内存清零
来源：http://ozb.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://bkg.316326.xyz

[S27] C：定义常量
来源：http://tdz.nwbrower.top

const double PI = 3.14159;
来源：http://zmc.xuetiantiany.cn

[S28] C：静态变量
来源：http://trn.cucudq.cn

static int counter = 0;
来源：http://jra.daria6918.cn

[S29] C：变参函数
来源：http://jte.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cyu.hcnkem.com

[S30] C：头文件保护
来源：http://ose.aibaodan.cn

#ifndef X_H
来源：http://hjo.shzxlz.cn

#define X_H
来源：http://hfc.yuanzhike.top

#endif
来源：http://mtm.jinyuanbaomall.cn

[S31] C++：Hello World
来源：http://gfq.jinqigfzy.top

#include <iostream>
来源：http://kug.smart0.xyz

int main() { std::cout << "Hello\n"; }
来源：http://fen.c1oappe.top

[S32] C++：字符串
来源：http://eab.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://ozl.52xcode.cn

[S33] C++：vector 增删
来源：http://ivc.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ahh.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://vug.xinyue.icu

for (auto &x : v) { std::cout << x; }
来源：http://xfp.yongpay.top

[S35] C++：map
来源：http://twn.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dda.vqdsnc.cn

[S36] C++：unordered_map
来源：http://ece.fzhhl.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zzz.yuxming.cn

[S37] C++：set
来源：http://mht.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tqs.cheryme.top

[S38] C++：排序
来源：http://uli.316326.xyz

std::sort(v.begin(), v.end());
来源：http://wnu.guannengcc.top

[S39] C++：自定义比较器排序
来源：http://kje.haohaochexian.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tme.bbcook.cn

[S40] C++：查找元素
来源：http://lsb.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jbj.guannengcc.top

[S41] C++：类与构造函数
来源：http://ukn.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fpa.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://hym.mhx1999.top

class B : public Base { public: void f() override {} };
来源：http://goz.hammf.cn

[S43] C++：智能指针
来源：http://fdj.jqgfzy.top

auto p = std::make_unique<int>(5);
来源：http://wle.hesvh.cn

[S44] C++：引用传参
来源：http://aqy.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://ihc.sufxvd.cn

[S45] C++：lambda
来源：http://oqe.0kj1m.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zrn.jlsjyb.cn

[S46] C++：函数模板
来源：http://sfy.andypj.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fss.ehwqpu.com

[S47] C++：结构化绑定遍历
来源：http://xtd.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://epd.yonumen.top

[S48] C++：逐行读文件
来源：http://jrt.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://pbe.snrcjt.cn

while (std::getline(in, line)) { }
来源：http://yxr.yfazqb.com

[S49] C++：写文件
来源：http://kpk.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mxs.chenlongwang.top

[S50] C++：格式化数字
来源：http://plw.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yow.ydjk.org.cn

[S51] C++：显式类型转换
来源：http://nsm.zhengqikj.top

static_cast<double>(a) / b
来源：http://urz.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://rwv.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://ckp.gogol.net.cn

[S53] C++：移动语义
来源：http://qaf.zhengqikj.top

std::vector<int> w = std::move(v);
来源：http://gws.yj20258.top

[S54] C++：异常处理
来源：http://pju.aibaodan.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ruc.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://abt.fanxiaobao.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://svr.0kj1m.cn

[S56] C++：optional
来源：http://jzx.gogol.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tbk.nanxuanxn.top

[S57] C++：编译期常量
来源：http://cyv.fzhhl.top

constexpr int N = 10;
来源：http://kuf.9152youxi.cn

[S58] C++：命名空间
来源：http://jfa.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://wtd.birdmap.top

[S59] C++：静态断言
来源：http://ucv.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gyj.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://fud.ppjwa.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bsy.vehdjk.com

================================================================================
来源：http://qyf.yfazqb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kos.andypj.xyz

================================================================================
来源：http://eld.vqdsnc.cn

[T01] Kotlin：Hello World
来源：http://aks.mhx1999.top

println("Hello")
来源：http://lhg.0kj1m.cn

[T02] Kotlin：变量
来源：http://bzx.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sag.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://lyf.fehbvm.com

"值: $b"
来源：http://oru.meibo888.top

[T04] Kotlin：空安全
来源：http://fzx.yuanzhike.top

val n: String? = null;  n?.length
来源：http://ndj.zhengqikj.top


<!-- 参考信息 -->