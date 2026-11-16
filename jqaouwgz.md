代发 wailian999

set -euo pipefail
来源：http://auq.xylfe.cn

[R02] 变量赋值与使用
来源：http://cco.quarkkingdee.top

name="Tom"; echo "$name"
来源：http://bjw.hysaishi.cn

[R03] 只读变量
来源：http://nds.mhx1999.top

readonly PI=3.14
来源：http://pjk.vehdjk.com

[R04] 位置参数
来源：http://kdb.tarul.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xgj.zycfv.cn

[R05] 参数默认值
来源：http://fzg.mhx1999.top

name="${1:-default}"
来源：http://wbc.svipenyu.cn

[R06] 判断命令是否存在
来源：http://gtu.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gsq.uphjek.com

[R07] if 判断文件
来源：http://giw.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jmg.pycfn.com

[R08] 数值比较
来源：http://sem.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cdb.meibo888.top

[R09] 字符串比较
来源：http://lrt.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lhq.yuanzhike.top

[R10] 正则匹配
来源：http://cyg.ehwqpu.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tyv.yongpay.top

[R11] case 多分支
来源：http://dli.jinyuanbaomall.cn

case "$1" in
来源：http://pza.zhaomingkeji.xyz

start) echo "启动" ;;
来源：http://qhj.cheryme.top

stop)  echo "停止" ;;
来源：http://oik.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://fsi.jinqigufen.top

esac
来源：http://bix.zhongyouzk.top

[R12] for 遍历文件
来源：http://ziu.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://ssp.guowangkeji.top

[R13] for 计数循环
来源：http://sem.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://jpp.wangdashe.top

[R14] C 风格 for
来源：http://zxu.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gux.gogol.net.cn

[R15] while 逐行读文件
来源：http://qsy.hfpthk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cfz.fengsongda.top

[R16] until 等待条件
来源：http://bbm.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tqh.xylfe.cn

[R17] 数组定义与取值
来源：http://hvg.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vzx.daxiang520.top

[R18] 遍历数组
来源：http://pmx.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qnd.fzhhl.top

[R19] 数组长度
来源：http://tfd.aizwys.cn

echo "${#arr[@]}"
来源：http://vvq.andypj.xyz

[R20] 关联数组（字典）
来源：http://ssq.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://erz.tarul.cn

[R21] 字符串长度
来源：http://hcf.bbcook.cn

echo "${#s}"
来源：http://swb.dianchejie.cn

[R22] 截取子串
来源：http://unn.ppjwa.cn

echo "${s:0:5}"
来源：http://gzw.smart0.xyz

[R23] 字符串替换
来源：http://zij.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sch.guowangkeji.top

[R24] 大小写转换
来源：http://jrd.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://uol.ehwqpu.com

[R25] 去后缀 / 去前缀
来源：http://sgx.fzhhl.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tsb.yueranfly.top

[R26] 命令替换
来源：http://fpa.ydjk.org.cn

now=$(date +%F); echo "$now"
来源：http://idr.vehdjk.com

[R27] 算术展开
来源：http://rzv.nanxuanxn.top

echo $((1 + 2 * 3))
来源：http://dio.jinqigfzy.top

[R28] 浮点运算
来源：http://sbq.tarul.cn

echo "scale=2; 10/3" | bc
来源：http://kqt.yj20258.top

[R29] 定义函数
来源：http://kvy.yvedp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zwh.pycfn.com

[R30] 函数返回状态码
来源：http://owq.cdnleiting.top

f() { return 0; }; f || echo "失败了"
来源：http://ewg.dashuyun.cn

[R31] 局部变量
来源：http://rmc.jianghu66.top

f() { local x=1; echo "$x"; }
来源：http://fhr.wangdashe.top

[R32] 参数个数校验
来源：http://tfa.jqgfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xbv.gzhubu.top

[R33] 捕获错误并提示行号
来源：http://qiw.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fwt.quarkkingdee.top

[R34] 退出时清理
来源：http://rps.zhaomingkeji.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://hzx.bjfxy.top

[R35] 后台执行并等待
来源：http://wuv.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vlj.zhixingplan.top

[R36] 并发执行多个任务
来源：http://nci.fehbvm.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dmq.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://pxk.xziqi.cn

files=$(ls -1)
来源：http://xss.jlsjyb.cn

[R38] 管道串联
来源：http://jbn.yueranfly.top

cat a.txt | grep -i error | wc -l
来源：http://ajb.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://fnk.jianghu66.top

cmd > out.log 2>&1
来源：http://hmp.zhaomingkeji.xyz

[R40] 追加写日志
来源：http://sih.fanxiaobao.xyz

echo "log" >> out.log
来源：http://dbx.xylfe.cn

[R41] 丢弃输出
来源：http://slh.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://foo.yonumen.top

[R42] 输入重定向
来源：http://xhq.nwbrower.top

wc -l < a.txt
来源：http://dck.zdbjq.cn

[R43] 按名字查找文件
来源：http://jjc.kuanghao11.cn

find . -name "*.log" -type f
来源：http://zxq.kuanghao11.cn

[R44] 按修改时间查找
来源：http://qfa.0kj1m.cn

find . -mtime -7 -type f
来源：http://tdy.shangyingyoupin.top

[R45] 批量删除
来源：http://dpi.xylfe.cn

find . -name "*.tmp" -delete
来源：http://xov.ehwqpu.com

[R46] 递归替换文件内容
来源：http://kum.dashuyun.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oja.yj20258.top

[R47] sed 单行替换
来源：http://rqd.dashuyun.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qgq.pengpengdd.cyou

[R48] awk 取指定列
来源：http://mhj.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://rbb.snrcjt.cn

[R49] awk 带条件
来源：http://vuy.cashguo.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hyu.sysykeji.top

[R50] awk 求和
来源：http://axd.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yol.316326.xyz

[R51] 排序去重取前几
来源：http://dbi.tanke756.top

sort a.txt | uniq -c | sort -rn | head
来源：http://yxk.wangdashe.top

[R52] 统计行数
来源：http://lsh.jqgufenzy.top

wc -l a.txt
来源：http://hxq.yj202588.top

[R53] 查看文件头与实时尾
来源：http://jtj.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fzl.yonumen.top

[R54] 比较两个文件
来源：http://wpm.jlsjyb.cn

diff a.txt b.txt
来源：http://obf.tanke756.top

[R55] 压缩与解压
来源：http://wga.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rrr.tanke756.top

[R56] 远程拷贝
来源：http://ado.redwolf501.top

scp file user@host:/path/
来源：http://ndc.shangyingyoupin.top

[R57] 远程执行命令
来源：http://cht.yj202588.top

ssh user@host 'uptime'
来源：http://lcs.gaohongyu789.top

[R58] 下载文件
来源：http://nxn.yonumen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pzj.zhijiandao.cn

[R59] 发 POST JSON
来源：http://wfx.zdqjudy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ept.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://fje.nanxinkj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://acg.0kj1m.cn

[R61] 磁盘占用
来源：http://tck.aizwys.cn

df -h;  du -sh *
来源：http://eke.bjfxy.top

[R62] 找最占空间的文件
来源：http://uos.snrcjt.cn

du -ah . | sort -rh | head -10
来源：http://aex.havefunace.top

[R63] 内存与进程
来源：http://mez.uphjek.com

free -h;  ps aux | grep nginx
来源：http://dck.cdnleiting.top

[R64] 结束进程
来源：http://ljw.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://iwv.iojbl.cn

[R65] 查看端口占用
来源：http://wha.hysaishi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xtx.uphjek.com

[R66] 定时任务
来源：http://tup.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://kho.mhx1999.top

[R67] 生成随机十六进制串
来源：http://sei.kuanghao11.cn

openssl rand -hex 16
来源：http://lzz.yueranfly.top

[R68] 计算文件校验值
来源：http://ykv.meibo888.top

sha256sum a.txt;  md5sum a.txt
来源：http://rrb.jqgufenzy.top

[R69] 生成随机密码
来源：http://nbi.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://xnm.bjfxy.top

[R70] 时间戳与互转
来源：http://vba.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://kwj.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://nbt.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fxq.fzhhl.top

[R72] 等待端口就绪
来源：http://wln.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nci.jinqigfzy.top

[R73] 分割大日志
来源：http://kdb.zhengqikj.top

split -l 1000 big.log part_
来源：http://msj.jinyuanbaomall.cn

[R74] 批量重命名
来源：http://bbz.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tcx.tarul.cn

[R75] 导出环境变量
来源：http://awz.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://kyh.0kj1m.cn

[R76] 使用临时文件
来源：http://cdw.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oec.fzhhl.top

[R77] 读取用户输入
来源：http://dcw.jiagoushi.top

read -rp "请输入: " ans
来源：http://qjq.aizwys.cn

[R78] 交互式菜单
来源：http://ogt.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bmo.hnqzz.top

[R79] 解析命令行选项
来源：http://dua.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://izq.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://sau.xylfe.cn

time ./run.sh
来源：http://ztj.vehdjk.com

================================================================================
来源：http://cnb.bbcook.cn

S. C / C++ 专题
来源：http://uml.yongpay.top

================================================================================
来源：http://axe.yuanzhike.top

[S01] C：Hello World
来源：http://gkl.zhengqikj.top

#include <stdio.h>
来源：http://cwz.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://jst.cheryme.top

[S02] C：变量与格式化输出
来源：http://lda.zhixingplan.top

int a = 10; printf("%d\n", a);
来源：http://ofg.tianlin.xyz

[S03] C：读入整数
来源：http://ias.cucudq.cn

int x; scanf("%d", &x);
来源：http://umg.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://tvm.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hle.ppjwa.cn

[S05] C：字符串长度
来源：http://wtm.wangdashe.top

strlen(s)
来源：http://iuh.pycfn.com

[S06] C：字符串比较
来源：http://naw.tian-w.cn

strcmp(a, b) == 0
来源：http://rkf.shuidangran.top

[S07] C：数组遍历求和
来源：http://hqy.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gnt.tarul.cn

[S08] C：动态内存分配与释放
来源：http://ncl.daria6918.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yxx.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://igh.pengpengdd.cyou

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://giq.fktsv.cn

[S10] C：指针与解引用
来源：http://ddg.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://ybw.mhx1999.top

[S11] C：逐行读文件
来源：http://dvg.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://ikk.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dcx.zhijiandao.cn

fclose(f);
来源：http://mpp.yfazqb.com

[S12] C：写文件
来源：http://vvu.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ept.zhijiandao.cn

[S13] C：宏定义
来源：http://tdc.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tah.zhiwuduotai.top

[S14] C：枚举
来源：http://yvg.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://are.pengpengdd.cyou

[S15] C：类型转换
来源：http://kyh.jyoumei.cn

(double) a / b
来源：http://cco.aizwys.cn

[S16] C：位操作置位
来源：http://hxt.hongshengwenyu.top

x |= (1 << 3);
来源：http://mse.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://owx.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bhk.tian-w.cn

[S18] C：命令行参数
来源：http://euk.gotoacloud.top

int main(int argc, char **argv)
来源：http://ssh.yangfankeji.com

[S19] C：快速排序
来源：http://wzu.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://tuz.jlsjyb.cn

[S20] C：二分查找
来源：http://pna.pengpengdd.cyou

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nft.yuxming.cn

[S21] C：字符类别判断
来源：http://vjg.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uhh.xziqi.cn

[S22] C：字符串转数字
来源：http://thi.jqgufenzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://gwd.hcnkem.com

[S23] C：随机数
来源：http://unb.ivvv.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ynu.yj202588.top

[S24] C：获取本地时间
来源：http://ofs.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://svi.birdmap.top

[S25] C：内存拷贝
来源：http://evh.dashuyun.cn

memcpy(dst, src, n);
来源：http://cqy.zhoulong.xyz

[S26] C：内存清零
来源：http://gvr.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://lwd.xuanzx.com

[S27] C：定义常量
来源：http://ijs.sufxvd.cn

const double PI = 3.14159;
来源：http://gwq.xuanzx.com

[S28] C：静态变量
来源：http://dck.redwolf501.top

static int counter = 0;
来源：http://tqh.haohaochexian.top

[S29] C：变参函数
来源：http://ttr.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://omm.birdmap.top

[S30] C：头文件保护
来源：http://guc.shanyushiyangtech.top

#ifndef X_H
来源：http://wve.fanxiaobao.xyz

#define X_H
来源：http://wyv.yj20258888.top

#endif
来源：http://vgg.fehbvm.com

[S31] C++：Hello World
来源：http://urd.smart0.xyz

#include <iostream>
来源：http://niq.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://kcx.yj202588.top

[S32] C++：字符串
来源：http://vsr.jlsjyb.cn

std::string s = "hi";  s += "!";
来源：http://ora.guowangkeji.top

[S33] C++：vector 增删
来源：http://mav.nanxuanxn.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://krh.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://oyy.sjlbkw.cn

for (auto &x : v) { std::cout << x; }
来源：http://dji.xingfuxueyuan.xyz

[S35] C++：map
来源：http://opb.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mtm.aibaodan.cn

[S36] C++：unordered_map
来源：http://fbb.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://paa.zhiwuduotai.top

[S37] C++：set
来源：http://cta.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ttf.snrcjt.cn

[S38] C++：排序
来源：http://qzz.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://xzv.jinyuanbaomall.cn

[S39] C++：自定义比较器排序
来源：http://daz.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yme.yongpay.top

[S40] C++：查找元素
来源：http://uwm.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://meb.vehdjk.com

[S41] C++：类与构造函数
来源：http://kvh.cashguo.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nhe.nanxinkj.top

[S42] C++：继承与虚函数
来源：http://lyy.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://htx.zdqjudy.top

[S43] C++：智能指针
来源：http://qvb.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://cwj.zycfv.cn

[S44] C++：引用传参
来源：http://otw.c1oappe.top

void inc(int &x) { ++x; }
来源：http://zni.316326.xyz

[S45] C++：lambda
来源：http://pgd.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://qqv.hnqzz.top

[S46] C++：函数模板
来源：http://fch.sweek.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://opf.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://ser.zhoulong.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vsf.jqgfzy.top

[S48] C++：逐行读文件
来源：http://gfm.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ijk.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://uml.wangshuangyany.cn

[S49] C++：写文件
来源：http://qhj.yj20258.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jes.ivvv.top

[S50] C++：格式化数字
来源：http://wxu.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pjy.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://afv.jqgufenzy.top

static_cast<double>(a) / b
来源：http://bkq.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://jfh.nanxuanxn.top

int size() const noexcept { return n_; }
来源：http://pli.wangdashe.top

[S53] C++：移动语义
来源：http://mjp.gotoacloud.top

std::vector<int> w = std::move(v);
来源：http://abc.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://glu.ppjwa.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xej.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://pvi.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fzj.tianlin.xyz

[S56] C++：optional
来源：http://tdx.jqgufenzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vdn.cashguo.top

[S57] C++：编译期常量
来源：http://oth.chenjidiqi.icu

constexpr int N = 10;
来源：http://zzd.yj20258888.top

[S58] C++：命名空间
来源：http://zkz.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://lyx.fzhhl.top

[S59] C++：静态断言
来源：http://ffd.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://krr.yongpay.top

[S60] C++：遍历并删除元素
来源：http://iub.yj202588.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://twy.0kj1m.cn

================================================================================
来源：http://qxn.wangdashe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ale.ybcxt.top

================================================================================
来源：http://fkt.xziqi.cn

[T01] Kotlin：Hello World
来源：http://yyb.cucudq.cn

println("Hello")
来源：http://wrf.ybcxt.top

[T02] Kotlin：变量
来源：http://xfs.haohaochexian.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fob.jinyuanbaomall.cn


<!-- 参考信息 -->