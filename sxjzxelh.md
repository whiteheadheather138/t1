代发 wailian999

readonly PI=3.14
来源：http://dnm.andypj.xyz

[R04] 位置参数
来源：http://lpi.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://muf.jqgufenzy.top

[R05] 参数默认值
来源：http://qrs.ydzc1.top

name="${1:-default}"
来源：http://vlk.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://too.yueranfly.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ssg.chenlongwang.top

[R07] if 判断文件
来源：http://mfj.9152youxi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://neb.shzxlz.cn

[R08] 数值比较
来源：http://dob.sxryk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fkm.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://slw.fengsongda.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uzq.chenjidiqi.icu

[R10] 正则匹配
来源：http://bll.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rgp.yj20258888.top

[R11] case 多分支
来源：http://jfy.zhixingplan.top

case "$1" in
来源：http://vnm.ydjk.org.cn

start) echo "启动" ;;
来源：http://omq.9152youxi.cn

stop)  echo "停止" ;;
来源：http://xyx.tanke756.top

*)     echo "未知命令" ;;
来源：http://xqr.zdbjq.cn

esac
来源：http://cry.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://oqx.zhijiandao.cn

for f in *.txt; do echo "$f"; done
来源：http://vno.jianghu66.top

[R13] for 计数循环
来源：http://nji.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://dle.yonumen.top

[R14] C 风格 for
来源：http://bmb.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kom.ybcxt.top

[R15] while 逐行读文件
来源：http://skx.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://orx.zdqjudy.top

[R16] until 等待条件
来源：http://ske.aibaodan.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xof.yongpay.top

[R17] 数组定义与取值
来源：http://ngr.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lrk.yongpay.top

[R18] 遍历数组
来源：http://ilh.yonumen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bgv.epnwcf.com

[R19] 数组长度
来源：http://qdl.9152youxi.cn

echo "${#arr[@]}"
来源：http://npn.9152youxi.cn

[R20] 关联数组（字典）
来源：http://hji.zhixingplan.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hgz.tarul.cn

[R21] 字符串长度
来源：http://hvl.zhiwuduotai.top

echo "${#s}"
来源：http://asl.zhoulong.xyz

[R22] 截取子串
来源：http://arh.havefunace.top

echo "${s:0:5}"
来源：http://nex.hysaishi.cn

[R23] 字符串替换
来源：http://cah.ydjk.org.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lzf.ydzc1.top

[R24] 大小写转换
来源：http://ypv.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://toq.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://voj.sweek.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ooi.wangshuangyany.cn

[R26] 命令替换
来源：http://sfm.bjfxy.top

now=$(date +%F); echo "$now"
来源：http://bxu.jinqigfzy.top

[R27] 算术展开
来源：http://gin.yangfankeji.com

echo $((1 + 2 * 3))
来源：http://opw.yangfankeji.com

[R28] 浮点运算
来源：http://fcf.daria6918.cn

echo "scale=2; 10/3" | bc
来源：http://wym.jlsjyb.cn

[R29] 定义函数
来源：http://rzh.fktsv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aih.pengpengdd.cyou

[R30] 函数返回状态码
来源：http://geo.dianchejie.cn

f() { return 0; }; f || echo "失败了"
来源：http://rlo.yvedp.cn

[R31] 局部变量
来源：http://fpo.316326.xyz

f() { local x=1; echo "$x"; }
来源：http://ktb.sysykeji.top

[R32] 参数个数校验
来源：http://uce.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rft.xuanzx.com

[R33] 捕获错误并提示行号
来源：http://bju.jinyuanbaomall.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vld.9152youxi.cn

[R34] 退出时清理
来源：http://gxz.yj202588.top

trap 'rm -f "$tmp"' EXIT
来源：http://peu.jinqigfzy.top

[R35] 后台执行并等待
来源：http://nfq.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wfa.ydzc1.top

[R36] 并发执行多个任务
来源：http://znr.9152youxi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cdo.ehwqpu.com

[R37] 把输出赋给变量
来源：http://bqn.yj20258.top

files=$(ls -1)
来源：http://cfq.tanke756.top

[R38] 管道串联
来源：http://ekl.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://agk.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://kpg.nanxuanxn.top

cmd > out.log 2>&1
来源：http://wyy.epnwcf.com

[R40] 追加写日志
来源：http://jrh.ydzc1.top

echo "log" >> out.log
来源：http://cyb.cashguo.top

[R41] 丢弃输出
来源：http://hva.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://wvz.zhixingplan.top

[R42] 输入重定向
来源：http://maq.ydjk.org.cn

wc -l < a.txt
来源：http://idl.yj20258888.top

[R43] 按名字查找文件
来源：http://hce.sjlbkw.cn

find . -name "*.log" -type f
来源：http://mbc.nanxinkj.top

[R44] 按修改时间查找
来源：http://rut.cheryme.top

find . -mtime -7 -type f
来源：http://rhz.sweek.top

[R45] 批量删除
来源：http://opt.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://vjs.cheryme.top

[R46] 递归替换文件内容
来源：http://xpi.hnxiangtu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://omo.dianchejie.cn

[R47] sed 单行替换
来源：http://txh.yuxming.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cvl.gaohongyu789.top

[R48] awk 取指定列
来源：http://heh.jianghu66.top

awk '{print $1, $3}' a.txt
来源：http://ehq.shuidangran.top

[R49] awk 带条件
来源：http://ygu.iojbl.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lcn.birdmap.top

[R50] awk 求和
来源：http://smo.jiagoushi.top

awk '{s += $2} END {print s}' a.txt
来源：http://jar.yuxming.cn

[R51] 排序去重取前几
来源：http://unp.yonumen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://aqs.bbcook.cn

[R52] 统计行数
来源：http://aet.zhengqikj.top

wc -l a.txt
来源：http://qfz.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://mhg.jianghu66.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fhg.gaohongyu789.top

[R54] 比较两个文件
来源：http://pex.wangshuangyany.cn

diff a.txt b.txt
来源：http://wva.zdqjudy.top

[R55] 压缩与解压
来源：http://shf.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lsn.ehwqpu.com

[R56] 远程拷贝
来源：http://uyb.cashguo.top

scp file user@host:/path/
来源：http://tix.9152youxi.cn

[R57] 远程执行命令
来源：http://xkb.hnxiangtu.top

ssh user@host 'uptime'
来源：http://iih.iojbl.cn

[R58] 下载文件
来源：http://zyl.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zlc.yuanzhike.top

[R59] 发 POST JSON
来源：http://qee.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dgt.yfazqb.com

[R60] 只看 HTTP 状态码
来源：http://xld.tian-w.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://meg.haohaochexian.top

[R61] 磁盘占用
来源：http://qpr.hcnkem.com

df -h;  du -sh *
来源：http://era.shanyushiyangtech.top

[R62] 找最占空间的文件
来源：http://kma.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://kcc.cqqwz.cn

[R63] 内存与进程
来源：http://hph.ivvv.top

free -h;  ps aux | grep nginx
来源：http://fyr.guowangkeji.top

[R64] 结束进程
来源：http://gsz.shzxlz.cn

kill -9 $(pgrep -f app.py)
来源：http://qai.xuetiantiany.cn

[R65] 查看端口占用
来源：http://hoq.9152youxi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mrr.fehbvm.com

[R66] 定时任务
来源：http://ome.cashguo.top

crontab -e;  crontab -l
来源：http://rnb.jianghu66.top

[R67] 生成随机十六进制串
来源：http://rqf.ybcxt.top

openssl rand -hex 16
来源：http://gfl.hammf.cn

[R68] 计算文件校验值
来源：http://ysc.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://zxx.aibaodan.cn

[R69] 生成随机密码
来源：http://wsa.cheryme.top

head -c 16 /dev/urandom | base64
来源：http://rzc.fehbvm.com

[R70] 时间戳与互转
来源：http://koh.svipenyu.cn

date +%s;  date -d @1700000000
来源：http://osf.smart0.xyz

[R71] 日期格式化
来源：http://ggy.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jtb.yfazqb.com

[R72] 等待端口就绪
来源：http://xph.sxryk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yjg.aibaodan.cn

[R73] 分割大日志
来源：http://yuo.52xcode.cn

split -l 1000 big.log part_
来源：http://hnp.meibo888.top

[R74] 批量重命名
来源：http://hvc.gaohongyu789.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pln.nwbrower.top

[R75] 导出环境变量
来源：http://fyu.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://goi.hywenlv.cn

[R76] 使用临时文件
来源：http://uhn.yuxming.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://phh.tanke756.top

[R77] 读取用户输入
来源：http://iee.sysykeji.top

read -rp "请输入: " ans
来源：http://eos.jlsjyb.cn

[R78] 交互式菜单
来源：http://ajz.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mkv.cucudq.cn

[R79] 解析命令行选项
来源：http://deg.yuanzhike.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qfg.hywenlv.cn

[R80] 查看脚本执行耗时
来源：http://rgp.cucudq.cn

time ./run.sh
来源：http://udw.fzhhl.top

================================================================================
来源：http://qeg.hnqzz.top

S. C / C++ 专题
来源：http://atn.gotoacloud.top

================================================================================
来源：http://enw.tian-w.cn

[S01] C：Hello World
来源：http://xsx.sweek.top

#include <stdio.h>
来源：http://tho.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qmd.yuanzhike.top

[S02] C：变量与格式化输出
来源：http://pku.kuanghao11.cn

int a = 10; printf("%d\n", a);
来源：http://fxo.xylfe.cn

[S03] C：读入整数
来源：http://miq.guowangkeji.top

int x; scanf("%d", &x);
来源：http://psl.chenjidiqi.icu

[S04] C：字符串复制
来源：http://zvi.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://uup.hnxiangtu.top

[S05] C：字符串长度
来源：http://wtd.fzhhl.top

strlen(s)
来源：http://dyz.bjfxy.top

[S06] C：字符串比较
来源：http://smw.cashguo.top

strcmp(a, b) == 0
来源：http://rxk.chenzaomai.com

[S07] C：数组遍历求和
来源：http://gxj.gaohongyu789.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jjd.shuidangran.top

[S08] C：动态内存分配与释放
来源：http://kkv.fzhhl.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://awo.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://oxi.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vdk.ctjpmb.com

[S10] C：指针与解引用
来源：http://lrc.hnqzz.top

int *p = &a;  *p = 5;
来源：http://iif.jinqigfzy.top

[S11] C：逐行读文件
来源：http://vue.havefunace.top

FILE *f = fopen("a.txt", "r");
来源：http://jma.ctjpmb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://aww.nanxuanxn.top

fclose(f);
来源：http://zxe.fktsv.cn

[S12] C：写文件
来源：http://fyu.jyoumei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yjk.epnwcf.com

[S13] C：宏定义
来源：http://yhf.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nii.havefunace.top

[S14] C：枚举
来源：http://klf.ydzc1.top

enum Color { RED, GREEN, BLUE };
来源：http://mkk.hnxiangtu.top

[S15] C：类型转换
来源：http://plo.hammf.cn

(double) a / b
来源：http://npd.gotoacloud.top

[S16] C：位操作置位
来源：http://ytr.feifeiyinyue.top

x |= (1 << 3);
来源：http://knf.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://cyi.birdmap.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cyk.dianchejie.cn

[S18] C：命令行参数
来源：http://evm.sufxvd.cn

int main(int argc, char **argv)
来源：http://hki.sweek.top

[S19] C：快速排序
来源：http://knt.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://xyl.yfazqb.com

[S20] C：二分查找
来源：http://uxl.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zzo.snrcjt.cn

[S21] C：字符类别判断
来源：http://hgl.gotoacloud.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qnt.316326.xyz

[S22] C：字符串转数字
来源：http://uqd.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://qwm.guowangkeji.top

[S23] C：随机数
来源：http://lje.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://aas.hywenlv.cn

[S24] C：获取本地时间
来源：http://eho.fzhhl.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jyk.sweek.top

[S25] C：内存拷贝
来源：http://vjd.shzxlz.cn

memcpy(dst, src, n);
来源：http://zub.birdmap.top

[S26] C：内存清零
来源：http://dgz.fzhhl.top

memset(a, 0, sizeof a);
来源：http://tpv.zhixingplan.top

[S27] C：定义常量
来源：http://xne.yvedp.cn

const double PI = 3.14159;
来源：http://zlp.hammf.cn

[S28] C：静态变量
来源：http://zeo.hammf.cn

static int counter = 0;
来源：http://tpl.yj20258888.top

[S29] C：变参函数
来源：http://abw.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sla.gaohongyu789.top

[S30] C：头文件保护
来源：http://kus.cdnleiting.top

#ifndef X_H
来源：http://ltj.tanke756.top

#define X_H
来源：http://ohs.shuidangran.top

#endif
来源：http://wrx.uphjek.com

[S31] C++：Hello World
来源：http://chr.ivvv.top

#include <iostream>
来源：http://dzs.tianlin.xyz

int main() { std::cout << "Hello\n"; }
来源：http://kva.zhaomingkeji.xyz

[S32] C++：字符串
来源：http://ela.pycfn.com

std::string s = "hi";  s += "!";
来源：http://mkf.tianlin.xyz

[S33] C++：vector 增删
来源：http://xnz.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://soe.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://eoo.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://qen.gaohongyu789.top

[S35] C++：map
来源：http://rso.hammf.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rae.smart0.xyz

[S36] C++：unordered_map
来源：http://nak.yvedp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cvq.jlsjyb.cn

[S37] C++：set
来源：http://wcb.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jcq.zhixingplan.top

[S38] C++：排序
来源：http://wju.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://kyx.yj202588.top

[S39] C++：自定义比较器排序
来源：http://acq.cdnleiting.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wvd.hywenlv.cn

[S40] C++：查找元素
来源：http://vuk.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hhe.fktsv.cn

[S41] C++：类与构造函数
来源：http://bxl.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sxl.tarul.cn

[S42] C++：继承与虚函数
来源：http://omb.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://xma.yuanzhike.top

[S43] C++：智能指针
来源：http://vpo.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://ryj.vehdjk.com

[S44] C++：引用传参
来源：http://pgt.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://sqe.tian-w.cn

[S45] C++：lambda
来源：http://qgo.fktsv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pbz.bjfxy.top

[S46] C++：函数模板
来源：http://sox.fehbvm.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gjl.yangfankeji.com

[S47] C++：结构化绑定遍历
来源：http://amc.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kgo.zhongyouzk.top

[S48] C++：逐行读文件
来源：http://jce.cdnleiting.top

std::ifstream in("a.txt");  std::string line;
来源：http://cbj.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://qbu.hysaishi.cn

[S49] C++：写文件
来源：http://xvy.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wfn.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://bbe.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ivs.hywenlv.cn

[S51] C++：显式类型转换
来源：http://tyq.nwbrower.top

static_cast<double>(a) / b
来源：http://rpq.tanke756.top

[S52] C++：const 与 noexcept
来源：http://amv.jianghu66.top

int size() const noexcept { return n_; }
来源：http://qbd.pycfn.com

[S53] C++：移动语义
来源：http://wpi.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://flv.yfazqb.com

[S54] C++：异常处理
来源：http://pjd.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qzp.hcnkem.com

[S55] C++：结构化绑定
来源：http://lmm.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://umz.bbcook.cn

[S56] C++：optional
来源：http://ars.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xna.pycfn.com

[S57] C++：编译期常量
来源：http://fku.zhijiandao.cn

constexpr int N = 10;
来源：http://bbk.fehbvm.com

[S58] C++：命名空间
来源：http://gwl.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://hzk.cashguo.top

[S59] C++：静态断言
来源：http://fjj.yuanzhike.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xvo.vehdjk.com

[S60] C++：遍历并删除元素
来源：http://twy.cdnleiting.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ofz.aibaodan.cn

================================================================================
来源：http://xcx.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cwv.jqgufenzy.top

================================================================================
来源：http://aeb.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://olt.smart0.xyz

println("Hello")
来源：http://ogc.xziqi.cn

[T02] Kotlin：变量
来源：http://xpw.xinyue.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qvw.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://eyl.yuanzhike.top

"值: $b"
来源：http://cnb.jinqigfzy.top

[T04] Kotlin：空安全
来源：http://gly.yj20258.top

val n: String? = null;  n?.length
来源：http://bif.bbcook.cn


<!-- 参考信息 -->