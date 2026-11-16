代发 wailian999

name="${1:-default}"
来源：http://yia.chenjidiqi.icu

[R06] 判断命令是否存在
来源：http://std.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rhx.hammf.cn

[R07] if 判断文件
来源：http://yvk.xylfe.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wug.shanyushiyangkeji.top

[R08] 数值比较
来源：http://ynz.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://kys.redwolf501.top

[R09] 字符串比较
来源：http://opw.hnqzz.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nfj.meibo888.top

[R10] 正则匹配
来源：http://uwc.smart0.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lxo.zhiwuduotai.top

[R11] case 多分支
来源：http://gcs.xziqi.cn

case "$1" in
来源：http://hxx.shangyingyoupin.top

start) echo "启动" ;;
来源：http://why.yfazqb.com

stop)  echo "停止" ;;
来源：http://ozx.smart0.xyz

*)     echo "未知命令" ;;
来源：http://vwx.andypj.xyz

esac
来源：http://bqm.epnwcf.com

[R12] for 遍历文件
来源：http://crh.dianchejie.cn

for f in *.txt; do echo "$f"; done
来源：http://xrn.cqqwz.cn

[R13] for 计数循环
来源：http://tss.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://jcg.aizwys.cn

[R14] C 风格 for
来源：http://axs.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qbw.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://nle.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ezx.zdqjudy.top

[R16] until 等待条件
来源：http://dfc.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gkn.jqgufenzy.top

[R17] 数组定义与取值
来源：http://uxl.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://zdf.hnqzz.top

[R18] 遍历数组
来源：http://ayn.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nlp.xuetiantiany.cn

[R19] 数组长度
来源：http://vuv.yuxming.cn

echo "${#arr[@]}"
来源：http://nrc.zhiwuduotai.top

[R20] 关联数组（字典）
来源：http://bta.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kif.kuanghao11.cn

[R21] 字符串长度
来源：http://tsw.c1oappe.top

echo "${#s}"
来源：http://kit.jinghuilouyu.cn

[R22] 截取子串
来源：http://fhx.zhongyouzk.top

echo "${s:0:5}"
来源：http://thy.jyoumei.cn

[R23] 字符串替换
来源：http://knf.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://neq.vqdsnc.cn

[R24] 大小写转换
来源：http://kdz.sufxvd.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zsu.nanxinkj.top

[R25] 去后缀 / 去前缀
来源：http://yxk.pycfn.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://wyc.hammf.cn

[R26] 命令替换
来源：http://ogz.zhixingplan.top

now=$(date +%F); echo "$now"
来源：http://wwq.mhx1999.top

[R27] 算术展开
来源：http://irl.birdmap.top

echo $((1 + 2 * 3))
来源：http://hka.fengsongda.top

[R28] 浮点运算
来源：http://eus.xziqi.cn

echo "scale=2; 10/3" | bc
来源：http://eem.fktsv.cn

[R29] 定义函数
来源：http://uyr.shanyushiyangtech.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hjt.yj20258888.top

[R30] 函数返回状态码
来源：http://ibs.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://fdq.yj202588.top

[R31] 局部变量
来源：http://ade.andypj.xyz

f() { local x=1; echo "$x"; }
来源：http://qdc.316326.xyz

[R32] 参数个数校验
来源：http://nmw.xuanzx.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bha.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://ecd.xziqi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://txx.vqdsnc.cn

[R34] 退出时清理
来源：http://rwg.jqgfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://buy.jianghu66.top

[R35] 后台执行并等待
来源：http://hql.shanyushiyangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hsh.zycfv.cn

[R36] 并发执行多个任务
来源：http://hzs.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tam.hesvh.cn

[R37] 把输出赋给变量
来源：http://dfk.shanyushiyangkeji.top

files=$(ls -1)
来源：http://tgh.hcnkem.com

[R38] 管道串联
来源：http://ohj.c1oappe.top

cat a.txt | grep -i error | wc -l
来源：http://iwz.hammf.cn

[R39] 重定向标准输出与错误
来源：http://qta.shuidangran.top

cmd > out.log 2>&1
来源：http://ftm.ctjpmb.com

[R40] 追加写日志
来源：http://imd.havefunace.top

echo "log" >> out.log
来源：http://fzb.vqdsnc.cn

[R41] 丢弃输出
来源：http://nqj.bjfxy.top

cmd >/dev/null 2>&1
来源：http://xwk.xuanzx.com

[R42] 输入重定向
来源：http://rxd.hysaishi.cn

wc -l < a.txt
来源：http://tsh.gotoacloud.top

[R43] 按名字查找文件
来源：http://rdi.feifeiyinyue.top

find . -name "*.log" -type f
来源：http://jaa.cheryme.top

[R44] 按修改时间查找
来源：http://kex.jiagoushi.top

find . -mtime -7 -type f
来源：http://jtj.smart0.xyz

[R45] 批量删除
来源：http://jmt.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://ydk.bjfxy.top

[R46] 递归替换文件内容
来源：http://ybf.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jhx.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://jam.ivvv.top

sed -i 's/foo/bar/g' a.txt
来源：http://ylj.birdmap.top

[R48] awk 取指定列
来源：http://fax.jqgufenzy.top

awk '{print $1, $3}' a.txt
来源：http://mtp.meibo888.top

[R49] awk 带条件
来源：http://bkq.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kgi.ppjwa.cn

[R50] awk 求和
来源：http://hfg.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://xvh.sysykeji.top

[R51] 排序去重取前几
来源：http://dss.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kaf.gzhubu.top

[R52] 统计行数
来源：http://tcs.jyoumei.cn

wc -l a.txt
来源：http://jbz.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://kyk.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fbh.jqgufenzy.top

[R54] 比较两个文件
来源：http://urg.birdmap.top

diff a.txt b.txt
来源：http://hnb.guannengcc.top

[R55] 压缩与解压
来源：http://rie.bjfxy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ted.tanke756.top

[R56] 远程拷贝
来源：http://bmn.hcnkem.com

scp file user@host:/path/
来源：http://pyt.sjlbkw.cn

[R57] 远程执行命令
来源：http://hcw.yongpay.top

ssh user@host 'uptime'
来源：http://xbe.zdbjq.cn

[R58] 下载文件
来源：http://mli.ppjwa.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ggc.cqqwz.cn

[R59] 发 POST JSON
来源：http://yva.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ark.aibaodan.cn

[R60] 只看 HTTP 状态码
来源：http://azd.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ftz.xuanzx.com

[R61] 磁盘占用
来源：http://mri.zdbjq.cn

df -h;  du -sh *
来源：http://wsc.ehwqpu.com

[R62] 找最占空间的文件
来源：http://fqw.hongshengwenyu.top

du -ah . | sort -rh | head -10
来源：http://xvr.zhaomingkeji.xyz

[R63] 内存与进程
来源：http://hti.zhaomingkeji.xyz

free -h;  ps aux | grep nginx
来源：http://oek.jinqigfzy.top

[R64] 结束进程
来源：http://tvl.yongpay.top

kill -9 $(pgrep -f app.py)
来源：http://iip.pycfn.com

[R65] 查看端口占用
来源：http://bna.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jda.quarkkingdee.top

[R66] 定时任务
来源：http://atn.ctjpmb.com

crontab -e;  crontab -l
来源：http://oqu.shanyushiyangkeji.top

[R67] 生成随机十六进制串
来源：http://yhw.dianchejie.cn

openssl rand -hex 16
来源：http://jdq.cucudq.cn

[R68] 计算文件校验值
来源：http://usy.sysykeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://wel.chenjidiqi.icu

[R69] 生成随机密码
来源：http://xhi.jqgufenzy.top

head -c 16 /dev/urandom | base64
来源：http://nny.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://ngr.xylfe.cn

date +%s;  date -d @1700000000
来源：http://cik.jinyuanbaomall.cn

[R71] 日期格式化
来源：http://ums.shangyingyoupin.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://uzb.yueranfly.top

[R72] 等待端口就绪
来源：http://oyw.jiagoushi.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qjp.xinyue.icu

[R73] 分割大日志
来源：http://unl.ehwqpu.com

split -l 1000 big.log part_
来源：http://tsw.tianlin.xyz

[R74] 批量重命名
来源：http://avf.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dap.ivvv.top

[R75] 导出环境变量
来源：http://wng.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://nmf.cdnleiting.top

[R76] 使用临时文件
来源：http://lha.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zgj.0kj1m.cn

[R77] 读取用户输入
来源：http://kes.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://hop.zdbjq.cn

[R78] 交互式菜单
来源：http://msw.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xai.hammf.cn

[R79] 解析命令行选项
来源：http://uhp.yanxiufei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://own.ivvv.top

[R80] 查看脚本执行耗时
来源：http://knm.yonumen.top

time ./run.sh
来源：http://vbf.gaohongyu789.top

================================================================================
来源：http://efd.shangyingyoupin.top

S. C / C++ 专题
来源：http://viv.gzhubu.top

================================================================================
来源：http://yxr.epnwcf.com

[S01] C：Hello World
来源：http://xjl.tian-w.cn

#include <stdio.h>
来源：http://oat.cucudq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zjl.hammf.cn

[S02] C：变量与格式化输出
来源：http://ird.jlsjyb.cn

int a = 10; printf("%d\n", a);
来源：http://ayz.sufxvd.cn

[S03] C：读入整数
来源：http://cii.cucudq.cn

int x; scanf("%d", &x);
来源：http://evc.yangfankeji.com

[S04] C：字符串复制
来源：http://ivs.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eap.gotoacloud.top

[S05] C：字符串长度
来源：http://kxt.9152youxi.cn

strlen(s)
来源：http://ibo.uphjek.com

[S06] C：字符串比较
来源：http://qzt.sufxvd.cn

strcmp(a, b) == 0
来源：http://lcc.yj202588.top

[S07] C：数组遍历求和
来源：http://ekb.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dsv.ivvv.top

[S08] C：动态内存分配与释放
来源：http://tns.hesvh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ajc.yj202588.top

[S09] C：结构体定义与初始化
来源：http://vbe.yuxming.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ivi.xingfuxueyuan.xyz

[S10] C：指针与解引用
来源：http://efg.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://uqc.guannengcc.top

[S11] C：逐行读文件
来源：http://sjn.shzxlz.cn

FILE *f = fopen("a.txt", "r");
来源：http://zdf.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lle.dashuyun.cn

fclose(f);
来源：http://qfz.xingfuxueyuan.xyz

[S12] C：写文件
来源：http://gzf.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ejl.jyoumei.cn

[S13] C：宏定义
来源：http://yvu.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fav.vqdsnc.cn

[S14] C：枚举
来源：http://xhp.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://xzh.nwbrower.top

[S15] C：类型转换
来源：http://ibb.9152youxi.cn

(double) a / b
来源：http://ktv.gaohongyu789.top

[S16] C：位操作置位
来源：http://jqc.cqqwz.cn

x |= (1 << 3);
来源：http://vqg.316326.xyz

[S17] C：安全拼接字符串
来源：http://gng.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://npa.redwolf501.top

[S18] C：命令行参数
来源：http://dtc.haohaochexian.top

int main(int argc, char **argv)
来源：http://wvn.sjlbkw.cn

[S19] C：快速排序
来源：http://yon.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tee.hfpthk.cn

[S20] C：二分查找
来源：http://rbq.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fzn.wangdashe.top

[S21] C：字符类别判断
来源：http://ufu.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gzt.bjfxy.top

[S22] C：字符串转数字
来源：http://jqw.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://vwy.yuxming.cn

[S23] C：随机数
来源：http://hvs.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tfs.haohaochexian.top

[S24] C：获取本地时间
来源：http://orh.cheryme.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kfv.jqgufenzy.top

[S25] C：内存拷贝
来源：http://yiv.wangdashe.top

memcpy(dst, src, n);
来源：http://efm.xuanzx.com

[S26] C：内存清零
来源：http://byn.birdmap.top

memset(a, 0, sizeof a);
来源：http://gpu.aibaodan.cn

[S27] C：定义常量
来源：http://xzr.zhengqikj.top

const double PI = 3.14159;
来源：http://cys.yuxming.cn

[S28] C：静态变量
来源：http://bhs.aizwys.cn

static int counter = 0;
来源：http://zxj.xuanzx.com

[S29] C：变参函数
来源：http://uwx.nanxuanxn.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://car.ctjpmb.com

[S30] C：头文件保护
来源：http://hjc.yangfankeji.com

#ifndef X_H
来源：http://itk.jinqigufen.top

#define X_H
来源：http://ivq.pengpengdd.cyou

#endif
来源：http://hjn.xylfe.cn

[S31] C++：Hello World
来源：http://tev.shanyushiyangtech.top

#include <iostream>
来源：http://jnv.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://bfk.sufxvd.cn

[S32] C++：字符串
来源：http://ycr.hammf.cn

std::string s = "hi";  s += "!";
来源：http://zly.zhijiandao.cn

[S33] C++：vector 增删
来源：http://mqd.ppjwa.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jcf.jinqigfzy.top

[S34] C++：遍历 vector
来源：http://poq.jinqigufen.top

for (auto &x : v) { std::cout << x; }
来源：http://hlo.ybcxt.top

[S35] C++：map
来源：http://qzs.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qpk.gaohongyu789.top

[S36] C++：unordered_map
来源：http://get.shzxlz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wkv.ivvv.top

[S37] C++：set
来源：http://quo.svipenyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nkm.ppjwa.cn

[S38] C++：排序
来源：http://mwx.yanxiufei.cn

std::sort(v.begin(), v.end());
来源：http://enn.sufxvd.cn

[S39] C++：自定义比较器排序
来源：http://chd.kuanghao11.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qsx.yj20258888.top

[S40] C++：查找元素
来源：http://luk.gaohongyu789.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://olj.xingfuxueyuan.xyz

[S41] C++：类与构造函数
来源：http://auc.epnwcf.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xzn.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://gww.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://kcs.fzhhl.top

[S43] C++：智能指针
来源：http://cvd.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://lbd.pengpengdd.cyou

[S44] C++：引用传参
来源：http://amb.nanxinkj.top

void inc(int &x) { ++x; }
来源：http://uwd.shanyushiyangtech.top

[S45] C++：lambda
来源：http://lam.jlsjyb.cn

auto add = [](int a, int b) { return a + b; };
来源：http://afa.shangyingyoupin.top

[S46] C++：函数模板
来源：http://rsc.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wqk.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://xws.tarul.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iel.sufxvd.cn

[S48] C++：逐行读文件
来源：http://xmo.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hal.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://khp.dashuyun.cn

[S49] C++：写文件
来源：http://sfu.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wlg.ybcxt.top

[S50] C++：格式化数字
来源：http://aey.zhongyouzk.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uyj.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://ljr.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://rrv.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://pgo.yj20258.top

int size() const noexcept { return n_; }
来源：http://mic.daxiang520.top

[S53] C++：移动语义
来源：http://qli.zhengqikj.top

std::vector<int> w = std::move(v);
来源：http://myp.iojbl.cn

[S54] C++：异常处理
来源：http://kwa.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ium.jqgufenzy.top

[S55] C++：结构化绑定
来源：http://woa.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mit.zhaomingkeji.xyz

[S56] C++：optional
来源：http://kvt.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aso.gotoacloud.top

[S57] C++：编译期常量
来源：http://imu.yj20258888.top

constexpr int N = 10;
来源：http://way.jianghu66.top

[S58] C++：命名空间
来源：http://ine.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://doi.jinghuilouyu.cn

[S59] C++：静态断言
来源：http://ynv.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aza.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://jyc.ppjwa.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yhj.iojbl.cn

================================================================================
来源：http://ags.c1oappe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yhs.yvedp.cn

================================================================================
来源：http://pej.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://gww.chenjidiqi.icu

println("Hello")
来源：http://enz.nanxinkj.top

[T02] Kotlin：变量
来源：http://bti.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uos.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://igb.vqdsnc.cn

"值: $b"
来源：http://nhd.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://bwr.iojbl.cn

val n: String? = null;  n?.length
来源：http://dbc.cqqwz.cn

[T05] Kotlin：when 表达式
来源：http://ity.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fte.ybcxt.top

[T06] Kotlin：集合映射
来源：http://nkx.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://iea.vehdjk.com


<!-- 参考信息 -->