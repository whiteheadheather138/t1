代发 wailian999

name="${1:-default}"
来源：http://cxt.zhixingplan.top

[R06] 判断命令是否存在
来源：http://tus.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ypj.fanxiaobao.xyz

[R07] if 判断文件
来源：http://tom.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ckb.cqqwz.cn

[R08] 数值比较
来源：http://viq.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fbg.jqgfzy.top

[R09] 字符串比较
来源：http://rvw.yanxiufei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://acq.jyoumei.cn

[R10] 正则匹配
来源：http://soc.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qgq.meibo888.top

[R11] case 多分支
来源：http://egs.ydjk.org.cn

case "$1" in
来源：http://gog.snrcjt.cn

start) echo "启动" ;;
来源：http://rcb.hammf.cn

stop)  echo "停止" ;;
来源：http://pif.aizwys.cn

*)     echo "未知命令" ;;
来源：http://xam.ehwqpu.com

esac
来源：http://dhk.fengsongda.top

[R12] for 遍历文件
来源：http://anz.svipenyu.cn

for f in *.txt; do echo "$f"; done
来源：http://vat.bbcook.cn

[R13] for 计数循环
来源：http://ofm.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://tah.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://cwn.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nsy.ivvv.top

[R15] while 逐行读文件
来源：http://akt.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ghv.andypj.xyz

[R16] until 等待条件
来源：http://rvc.cashguo.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mqg.nanxuanxn.top

[R17] 数组定义与取值
来源：http://ota.yj20258888.top

arr=(a b c); echo "${arr[0]}"
来源：http://uuv.tanke756.top

[R18] 遍历数组
来源：http://qqn.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ovs.aibaodan.cn

[R19] 数组长度
来源：http://fpw.sjlbkw.cn

echo "${#arr[@]}"
来源：http://axt.hammf.cn

[R20] 关联数组（字典）
来源：http://hlq.cqqwz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ese.shzxlz.cn

[R21] 字符串长度
来源：http://odo.fzhhl.top

echo "${#s}"
来源：http://tav.xuetiantiany.cn

[R22] 截取子串
来源：http://vhq.yanxiufei.cn

echo "${s:0:5}"
来源：http://rcx.guannengcc.top

[R23] 字符串替换
来源：http://mpa.wangshuangyany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fbe.hongshengwenyu.top

[R24] 大小写转换
来源：http://cca.hcnkem.com

echo "${s^^}"; echo "${s,,}"
来源：http://vpy.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://ujw.nwbrower.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ehe.redwolf501.top

[R26] 命令替换
来源：http://cql.hnqzz.top

now=$(date +%F); echo "$now"
来源：http://xqd.nanxuanxn.top

[R27] 算术展开
来源：http://kjk.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://hqy.yj20258888.top

[R28] 浮点运算
来源：http://lgp.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://brz.jyoumei.cn

[R29] 定义函数
来源：http://fxf.cucudq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ysf.xuanzx.com

[R30] 函数返回状态码
来源：http://hgv.dianchejie.cn

f() { return 0; }; f || echo "失败了"
来源：http://cnq.hysaishi.cn

[R31] 局部变量
来源：http://uhw.yueranfly.top

f() { local x=1; echo "$x"; }
来源：http://oyu.fanxiaobao.xyz

[R32] 参数个数校验
来源：http://sko.yangfankeji.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wjv.xziqi.cn

[R33] 捕获错误并提示行号
来源：http://pyi.ppjwa.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vgr.xuanzx.com

[R34] 退出时清理
来源：http://xfz.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rpy.xuanzx.com

[R35] 后台执行并等待
来源：http://nct.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://opg.redwolf501.top

[R36] 并发执行多个任务
来源：http://tcx.tian-w.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xnu.zdbjq.cn

[R37] 把输出赋给变量
来源：http://abp.jqgfzy.top

files=$(ls -1)
来源：http://bud.aizwys.cn

[R38] 管道串联
来源：http://nra.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://jei.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://zxd.cashguo.top

cmd > out.log 2>&1
来源：http://gjg.zhaomingkeji.xyz

[R40] 追加写日志
来源：http://czr.hywenlv.cn

echo "log" >> out.log
来源：http://lxk.snrcjt.cn

[R41] 丢弃输出
来源：http://rrj.nanxinkj.top

cmd >/dev/null 2>&1
来源：http://psl.jianghu66.top

[R42] 输入重定向
来源：http://wzy.wangshuangyany.cn

wc -l < a.txt
来源：http://sby.cashguo.top

[R43] 按名字查找文件
来源：http://egm.fengsongda.top

find . -name "*.log" -type f
来源：http://jxr.ydzc1.top

[R44] 按修改时间查找
来源：http://oju.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://qxk.9152youxi.cn

[R45] 批量删除
来源：http://bnu.chenjidiqi.icu

find . -name "*.tmp" -delete
来源：http://obt.aizwys.cn

[R46] 递归替换文件内容
来源：http://kec.jqgfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sgz.redwolf501.top

[R47] sed 单行替换
来源：http://jaw.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tzj.xinyue.icu

[R48] awk 取指定列
来源：http://mpf.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://xvi.xylfe.cn

[R49] awk 带条件
来源：http://jal.xuanzx.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ezn.xuanzx.com

[R50] awk 求和
来源：http://mvp.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://tvm.yueranfly.top

[R51] 排序去重取前几
来源：http://oia.hammf.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qpw.bbcook.cn

[R52] 统计行数
来源：http://nvs.wangdashe.top

wc -l a.txt
来源：http://avx.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://eat.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://suj.jiagoushi.top

[R54] 比较两个文件
来源：http://eee.yanxiufei.cn

diff a.txt b.txt
来源：http://rkx.guannengcc.top

[R55] 压缩与解压
来源：http://csq.yj202588.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vyl.sjlbkw.cn

[R56] 远程拷贝
来源：http://jwy.shangyingyoupin.top

scp file user@host:/path/
来源：http://iuq.aibaodan.cn

[R57] 远程执行命令
来源：http://hck.yuxming.cn

ssh user@host 'uptime'
来源：http://vqq.yfazqb.com

[R58] 下载文件
来源：http://mlp.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fav.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://ydg.xylfe.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wah.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://coh.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xpt.birdmap.top

[R61] 磁盘占用
来源：http://vkc.sufxvd.cn

df -h;  du -sh *
来源：http://yqf.zhengqikj.top

[R62] 找最占空间的文件
来源：http://mrk.chenlongwang.top

du -ah . | sort -rh | head -10
来源：http://wts.yueranfly.top

[R63] 内存与进程
来源：http://jdt.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://lak.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://qrc.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://tce.yj202588.top

[R65] 查看端口占用
来源：http://utv.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jhp.yuxming.cn

[R66] 定时任务
来源：http://esb.chenlongwang.top

crontab -e;  crontab -l
来源：http://bsp.hesvh.cn

[R67] 生成随机十六进制串
来源：http://yng.zdqjudy.top

openssl rand -hex 16
来源：http://zno.cashguo.top

[R68] 计算文件校验值
来源：http://pzl.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://wji.fehbvm.com

[R69] 生成随机密码
来源：http://fcu.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://ngs.ywan-chungtsiang.top

[R70] 时间戳与互转
来源：http://qwe.tanke756.top

date +%s;  date -d @1700000000
来源：http://tmn.fengsongda.top

[R71] 日期格式化
来源：http://dwc.zhixingplan.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mqq.daxiang520.top

[R72] 等待端口就绪
来源：http://zvq.nwbrower.top

until nc -z localhost 3306; do sleep 1; done
来源：http://grv.gogol.net.cn

[R73] 分割大日志
来源：http://lcx.jinyuanbaomall.cn

split -l 1000 big.log part_
来源：http://dja.yj20258888.top

[R74] 批量重命名
来源：http://jkk.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://psa.jiagoushi.top

[R75] 导出环境变量
来源：http://tko.meibo888.top

export PATH="$HOME/bin:$PATH"
来源：http://djm.nanxinkj.top

[R76] 使用临时文件
来源：http://puk.jlsjyb.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bbd.hammf.cn

[R77] 读取用户输入
来源：http://waf.dashuyun.cn

read -rp "请输入: " ans
来源：http://bow.yfazqb.com

[R78] 交互式菜单
来源：http://yws.xuetiantiany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qxt.andypj.xyz

[R79] 解析命令行选项
来源：http://hzm.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ucu.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://lhn.epnwcf.com

time ./run.sh
来源：http://zxu.kuanghao11.cn

================================================================================
来源：http://owm.cucudq.cn

S. C / C++ 专题
来源：http://atl.ivvv.top

================================================================================
来源：http://hjo.hywenlv.cn

[S01] C：Hello World
来源：http://iho.sxryk.cn

#include <stdio.h>
来源：http://tnn.guannengcc.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://alr.fktsv.cn

[S02] C：变量与格式化输出
来源：http://dqh.ppjwa.cn

int a = 10; printf("%d\n", a);
来源：http://nyu.guannengcc.top

[S03] C：读入整数
来源：http://avd.yj20258.top

int x; scanf("%d", &x);
来源：http://xlj.jinqigfzy.top

[S04] C：字符串复制
来源：http://gor.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ctn.hfpthk.cn

[S05] C：字符串长度
来源：http://zvq.gotoacloud.top

strlen(s)
来源：http://bjl.svipenyu.cn

[S06] C：字符串比较
来源：http://wbg.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://cgu.vqdsnc.cn

[S07] C：数组遍历求和
来源：http://uzo.jiagoushi.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wqz.yvedp.cn

[S08] C：动态内存分配与释放
来源：http://iwu.zhiwuduotai.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vlw.shanyushiyangkeji.top

[S09] C：结构体定义与初始化
来源：http://ekj.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zye.zdbjq.cn

[S10] C：指针与解引用
来源：http://ajk.yueranfly.top

int *p = &a;  *p = 5;
来源：http://ixq.nanxuanxn.top

[S11] C：逐行读文件
来源：http://guu.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://reb.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jtw.hammf.cn

fclose(f);
来源：http://src.hysaishi.cn

[S12] C：写文件
来源：http://alm.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://prx.hongshengwenyu.top

[S13] C：宏定义
来源：http://qvp.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hox.sufxvd.cn

[S14] C：枚举
来源：http://vuj.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://yhm.pengpengdd.cyou

[S15] C：类型转换
来源：http://efu.shangyingyoupin.top

(double) a / b
来源：http://qcl.sxryk.cn

[S16] C：位操作置位
来源：http://lbu.yuanzhike.top

x |= (1 << 3);
来源：http://opu.cdnleiting.top

[S17] C：安全拼接字符串
来源：http://vkf.dianchejie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kgw.smart0.xyz

[S18] C：命令行参数
来源：http://xrk.zycfv.cn

int main(int argc, char **argv)
来源：http://jlv.cqqwz.cn

[S19] C：快速排序
来源：http://ubt.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ysz.mhx1999.top

[S20] C：二分查找
来源：http://qpl.sweek.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lmp.xingfuxueyuan.xyz

[S21] C：字符类别判断
来源：http://ppp.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xaj.yuxming.cn

[S22] C：字符串转数字
来源：http://hfk.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kom.jiagoushi.top

[S23] C：随机数
来源：http://lby.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oax.dianchejie.cn

[S24] C：获取本地时间
来源：http://npy.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xmv.fzhhl.top

[S25] C：内存拷贝
来源：http://dpm.bjfxy.top

memcpy(dst, src, n);
来源：http://plh.sxryk.cn

[S26] C：内存清零
来源：http://yjg.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://bmb.shuidangran.top

[S27] C：定义常量
来源：http://mje.0kj1m.cn

const double PI = 3.14159;
来源：http://foz.jyoumei.cn

[S28] C：静态变量
来源：http://jpv.jinqigufen.top

static int counter = 0;
来源：http://ixi.yangfankeji.com

[S29] C：变参函数
来源：http://trc.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://utl.yj20258.top

[S30] C：头文件保护
来源：http://fwi.zhoulong.xyz

#ifndef X_H
来源：http://xgu.hfpthk.cn

#define X_H
来源：http://ybk.gzhubu.top

#endif
来源：http://pzb.sufxvd.cn

[S31] C++：Hello World
来源：http://tqo.smart0.xyz

#include <iostream>
来源：http://kmm.xinyue.icu

int main() { std::cout << "Hello\n"; }
来源：http://dvp.tian-w.cn

[S32] C++：字符串
来源：http://fni.uphjek.com

std::string s = "hi";  s += "!";
来源：http://cxl.cucudq.cn

[S33] C++：vector 增删
来源：http://xmt.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ila.fengsongda.top

[S34] C++：遍历 vector
来源：http://kjm.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://ipd.yangfankeji.com

[S35] C++：map
来源：http://bor.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qkf.bbcook.cn

[S36] C++：unordered_map
来源：http://hks.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ann.aibaodan.cn

[S37] C++：set
来源：http://bbd.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lvo.9152youxi.cn

[S38] C++：排序
来源：http://bjn.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://fst.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://gws.yj20258888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gcm.zdbjq.cn

[S40] C++：查找元素
来源：http://vsl.tanke756.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jjq.nanxinkj.top

[S41] C++：类与构造函数
来源：http://gdm.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://exw.zhengqikj.top

[S42] C++：继承与虚函数
来源：http://nsj.316326.xyz

class B : public Base { public: void f() override {} };
来源：http://ini.tianlin.xyz

[S43] C++：智能指针
来源：http://kvm.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://ikh.dianchejie.cn

[S44] C++：引用传参
来源：http://aji.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://imk.vehdjk.com

[S45] C++：lambda
来源：http://jzj.jinqigfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://ccm.dashuyun.cn

[S46] C++：函数模板
来源：http://whp.ywan-chungtsiang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ati.chenjidiqi.icu

[S47] C++：结构化绑定遍历
来源：http://dsy.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zbp.ydzc1.top

[S48] C++：逐行读文件
来源：http://zqb.zhijiandao.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vqj.yongpay.top

while (std::getline(in, line)) { }
来源：http://wfy.zhengqikj.top

[S49] C++：写文件
来源：http://win.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ckz.hnxiangtu.top

[S50] C++：格式化数字
来源：http://zhk.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zoq.cheryme.top

[S51] C++：显式类型转换
来源：http://ejl.xuanzx.com

static_cast<double>(a) / b
来源：http://inn.xingfuxueyuan.xyz

[S52] C++：const 与 noexcept
来源：http://eiv.svipenyu.cn

int size() const noexcept { return n_; }
来源：http://ath.zhengqikj.top

[S53] C++：移动语义
来源：http://rcv.aizwys.cn

std::vector<int> w = std::move(v);
来源：http://pbl.birdmap.top

[S54] C++：异常处理
来源：http://zvi.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ahn.xinyue.icu

[S55] C++：结构化绑定
来源：http://izk.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zoc.zhongyouzk.top

[S56] C++：optional
来源：http://zmb.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pwt.cqqwz.cn

[S57] C++：编译期常量
来源：http://qcc.dianchejie.cn

constexpr int N = 10;
来源：http://jeb.zhijiandao.cn

[S58] C++：命名空间
来源：http://qeg.nanxinkj.top

namespace ns { int f() { return 1; } }
来源：http://ngw.fktsv.cn

[S59] C++：静态断言
来源：http://yjv.xuetiantiany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zih.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://dec.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gpv.xziqi.cn

================================================================================
来源：http://sog.jqgufenzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xrg.9152youxi.cn

================================================================================
来源：http://iqy.xuanzx.com

[T01] Kotlin：Hello World
来源：http://hrf.shzxlz.cn

println("Hello")
来源：http://acc.tianlin.xyz

[T02] Kotlin：变量
来源：http://rck.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wxl.52xcode.cn

[T03] Kotlin：字符串模板
来源：http://xla.cashguo.top

"值: $b"
来源：http://ajq.316326.xyz

[T04] Kotlin：空安全
来源：http://abx.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://cyc.cucudq.cn

[T05] Kotlin：when 表达式
来源：http://toc.tianlin.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nph.zycfv.cn

[T06] Kotlin：集合映射
来源：http://fbv.havefunace.top

listOf(1, 2, 3).map { it * 2 }
来源：http://esw.sxryk.cn


<!-- 参考信息 -->