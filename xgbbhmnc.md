代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vpv.zycfv.cn

[R08] 数值比较
来源：http://aah.cdnleiting.top

if (( a > b )); then echo "a 更大"; fi
来源：http://due.guowangkeji.top

[R09] 字符串比较
来源：http://ctg.snrcjt.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pnh.dianchejie.cn

[R10] 正则匹配
来源：http://wii.hongshengwenyu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://isw.sjlbkw.cn

[R11] case 多分支
来源：http://idw.yongpay.top

case "$1" in
来源：http://ljp.ydjk.org.cn

start) echo "启动" ;;
来源：http://bje.nwbrower.top

stop)  echo "停止" ;;
来源：http://vcy.yanxiufei.cn

*)     echo "未知命令" ;;
来源：http://sit.nwbrower.top

esac
来源：http://mee.zhijiandao.cn

[R12] for 遍历文件
来源：http://xhb.zhiwuduotai.top

for f in *.txt; do echo "$f"; done
来源：http://ghd.havefunace.top

[R13] for 计数循环
来源：http://dmq.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://mnd.shangyingyoupin.top

[R14] C 风格 for
来源：http://jgv.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xng.xylfe.cn

[R15] while 逐行读文件
来源：http://vwt.xingfuxueyuan.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wis.ydzc1.top

[R16] until 等待条件
来源：http://zmy.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vdn.nwbrower.top

[R17] 数组定义与取值
来源：http://fmv.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gxw.jinqigufen.top

[R18] 遍历数组
来源：http://mtu.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://udz.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://fcc.0kj1m.cn

echo "${#arr[@]}"
来源：http://qtj.jqgfzy.top

[R20] 关联数组（字典）
来源：http://dvg.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wwt.yj20258888.top

[R21] 字符串长度
来源：http://jcb.yuanzhike.top

echo "${#s}"
来源：http://ngl.tian-w.cn

[R22] 截取子串
来源：http://yol.ybcxt.top

echo "${s:0:5}"
来源：http://lhc.ydjk.org.cn

[R23] 字符串替换
来源：http://ueq.ybcxt.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hlb.jinqigfzy.top

[R24] 大小写转换
来源：http://qtj.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://upx.hnxiangtu.top

[R25] 去后缀 / 去前缀
来源：http://uvv.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pzl.jinyuanbaomall.cn

[R26] 命令替换
来源：http://zyq.sysykeji.top

now=$(date +%F); echo "$now"
来源：http://vfw.jinyuanbaomall.cn

[R27] 算术展开
来源：http://wgr.ctjpmb.com

echo $((1 + 2 * 3))
来源：http://fte.nwbrower.top

[R28] 浮点运算
来源：http://ryf.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://jku.hcnkem.com

[R29] 定义函数
来源：http://bkm.yuanzhike.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ido.nanxinkj.top

[R30] 函数返回状态码
来源：http://nvs.fzhhl.top

f() { return 0; }; f || echo "失败了"
来源：http://tvg.tian-w.cn

[R31] 局部变量
来源：http://pqn.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://wco.feifeiyinyue.top

[R32] 参数个数校验
来源：http://lcb.ctjpmb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iju.cashguo.top

[R33] 捕获错误并提示行号
来源：http://kkh.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ruh.chenjidiqi.icu

[R34] 退出时清理
来源：http://knn.hesvh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dmu.zhijiandao.cn

[R35] 后台执行并等待
来源：http://las.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vle.ivvv.top

[R36] 并发执行多个任务
来源：http://hrl.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sow.mhx1999.top

[R37] 把输出赋给变量
来源：http://las.aibaodan.cn

files=$(ls -1)
来源：http://qpx.hnxiangtu.top

[R38] 管道串联
来源：http://ypt.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://jhu.zhoulong.xyz

[R39] 重定向标准输出与错误
来源：http://dsm.nwbrower.top

cmd > out.log 2>&1
来源：http://ifq.zhijiandao.cn

[R40] 追加写日志
来源：http://cme.yvedp.cn

echo "log" >> out.log
来源：http://bfa.gotoacloud.top

[R41] 丢弃输出
来源：http://olk.vqdsnc.cn

cmd >/dev/null 2>&1
来源：http://aqi.iojbl.cn

[R42] 输入重定向
来源：http://vgo.hesvh.cn

wc -l < a.txt
来源：http://vdu.ydzc1.top

[R43] 按名字查找文件
来源：http://iin.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://ndi.yj20258888.top

[R44] 按修改时间查找
来源：http://roo.ydjk.org.cn

find . -mtime -7 -type f
来源：http://qpy.jlsjyb.cn

[R45] 批量删除
来源：http://hwo.ctjpmb.com

find . -name "*.tmp" -delete
来源：http://cgt.yongpay.top

[R46] 递归替换文件内容
来源：http://glf.zhongyouzk.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fbn.xziqi.cn

[R47] sed 单行替换
来源：http://gqg.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bot.pycfn.com

[R48] awk 取指定列
来源：http://mik.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://xex.nwbrower.top

[R49] awk 带条件
来源：http://vcz.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lgp.sxryk.cn

[R50] awk 求和
来源：http://wii.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://nmw.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://gju.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jnq.c1oappe.top

[R52] 统计行数
来源：http://fxo.chenzaomai.com

wc -l a.txt
来源：http://vdd.cucudq.cn

[R53] 查看文件头与实时尾
来源：http://lbs.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oov.uphjek.com

[R54] 比较两个文件
来源：http://vgc.haohaochexian.top

diff a.txt b.txt
来源：http://pim.fehbvm.com

[R55] 压缩与解压
来源：http://wyp.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wwn.yj20258888.top

[R56] 远程拷贝
来源：http://uqa.sjlbkw.cn

scp file user@host:/path/
来源：http://sfe.cashguo.top

[R57] 远程执行命令
来源：http://fza.tarul.cn

ssh user@host 'uptime'
来源：http://gsa.zhijiandao.cn

[R58] 下载文件
来源：http://isn.tianlin.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wtp.pycfn.com

[R59] 发 POST JSON
来源：http://amn.52xcode.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nli.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://cte.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kgo.xinyue.icu

[R61] 磁盘占用
来源：http://pln.zhengqikj.top

df -h;  du -sh *
来源：http://gku.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://vew.vehdjk.com

du -ah . | sort -rh | head -10
来源：http://ybd.iojbl.cn

[R63] 内存与进程
来源：http://ysm.gogol.net.cn

free -h;  ps aux | grep nginx
来源：http://idk.ydzc1.top

[R64] 结束进程
来源：http://bai.bbcook.cn

kill -9 $(pgrep -f app.py)
来源：http://rwn.xziqi.cn

[R65] 查看端口占用
来源：http://irg.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://flj.hysaishi.cn

[R66] 定时任务
来源：http://dut.guannengcc.top

crontab -e;  crontab -l
来源：http://mkc.cashguo.top

[R67] 生成随机十六进制串
来源：http://crt.sxryk.cn

openssl rand -hex 16
来源：http://tye.shangyingyoupin.top

[R68] 计算文件校验值
来源：http://hge.fzhhl.top

sha256sum a.txt;  md5sum a.txt
来源：http://uej.feifeiyinyue.top

[R69] 生成随机密码
来源：http://qpy.jyoumei.cn

head -c 16 /dev/urandom | base64
来源：http://cit.gogol.net.cn

[R70] 时间戳与互转
来源：http://vcx.zhongyouzk.top

date +%s;  date -d @1700000000
来源：http://jyv.jinyuanbaomall.cn

[R71] 日期格式化
来源：http://dey.wangdashe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wdm.ydzc1.top

[R72] 等待端口就绪
来源：http://abp.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kjp.jlsjyb.cn

[R73] 分割大日志
来源：http://gwj.sysykeji.top

split -l 1000 big.log part_
来源：http://ums.yangfankeji.com

[R74] 批量重命名
来源：http://ibn.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://drr.ehwqpu.com

[R75] 导出环境变量
来源：http://mfx.shanyushiyangtech.top

export PATH="$HOME/bin:$PATH"
来源：http://gzq.fehbvm.com

[R76] 使用临时文件
来源：http://oak.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fyv.daxiang520.top

[R77] 读取用户输入
来源：http://var.kuanghao11.cn

read -rp "请输入: " ans
来源：http://zjb.hcnkem.com

[R78] 交互式菜单
来源：http://ybi.jlsjyb.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mhw.sjlbkw.cn

[R79] 解析命令行选项
来源：http://str.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mqb.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://ucm.redwolf501.top

time ./run.sh
来源：http://opc.xylfe.cn

================================================================================
来源：http://hrs.yueranfly.top

S. C / C++ 专题
来源：http://xel.shanyushiyangtech.top

================================================================================
来源：http://kxj.jianghu66.top

[S01] C：Hello World
来源：http://rga.nanxinkj.top

#include <stdio.h>
来源：http://sdm.guannengcc.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jxb.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://pux.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://uwo.yanxiufei.cn

[S03] C：读入整数
来源：http://vqt.shangyingyoupin.top

int x; scanf("%d", &x);
来源：http://wcr.dashuyun.cn

[S04] C：字符串复制
来源：http://mbd.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://ldn.fehbvm.com

[S05] C：字符串长度
来源：http://uvy.zhixingplan.top

strlen(s)
来源：http://kvu.chenlongwang.top

[S06] C：字符串比较
来源：http://evk.nanxuanxn.top

strcmp(a, b) == 0
来源：http://nju.epnwcf.com

[S07] C：数组遍历求和
来源：http://eig.hnxiangtu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ymi.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://stj.daria6918.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://emm.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://rdg.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nrp.tian-w.cn

[S10] C：指针与解引用
来源：http://gnr.vehdjk.com

int *p = &a;  *p = 5;
来源：http://opa.ybcxt.top

[S11] C：逐行读文件
来源：http://svr.cheryme.top

FILE *f = fopen("a.txt", "r");
来源：http://yjz.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://hhn.xuanzx.com

fclose(f);
来源：http://vft.yfazqb.com

[S12] C：写文件
来源：http://das.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ekx.cqqwz.cn

[S13] C：宏定义
来源：http://pqx.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oun.ehwqpu.com

[S14] C：枚举
来源：http://okp.jinqigfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://poy.quarkkingdee.top

[S15] C：类型转换
来源：http://ilj.xingfuxueyuan.xyz

(double) a / b
来源：http://rkv.hongshengwenyu.top

[S16] C：位操作置位
来源：http://egg.uphjek.com

x |= (1 << 3);
来源：http://muq.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://igu.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hwe.feifeiyinyue.top

[S18] C：命令行参数
来源：http://kar.0kj1m.cn

int main(int argc, char **argv)
来源：http://nzd.svipenyu.cn

[S19] C：快速排序
来源：http://joi.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://xhc.cqqwz.cn

[S20] C：二分查找
来源：http://exq.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oll.andypj.xyz

[S21] C：字符类别判断
来源：http://fng.aibaodan.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://szz.bjfxy.top

[S22] C：字符串转数字
来源：http://hpg.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://gif.0kj1m.cn

[S23] C：随机数
来源：http://big.nanxuanxn.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xva.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://ozm.svipenyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ewi.gogol.net.cn

[S25] C：内存拷贝
来源：http://taw.yj202588.top

memcpy(dst, src, n);
来源：http://qbk.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://wwm.yj202588.top

memset(a, 0, sizeof a);
来源：http://gia.smart0.xyz

[S27] C：定义常量
来源：http://tru.aibaodan.cn

const double PI = 3.14159;
来源：http://qdq.xingfuxueyuan.xyz

[S28] C：静态变量
来源：http://gyz.xylfe.cn

static int counter = 0;
来源：http://pqw.zhoulong.xyz

[S29] C：变参函数
来源：http://vep.ehwqpu.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ybh.daxiang520.top

[S30] C：头文件保护
来源：http://oaz.yongpay.top

#ifndef X_H
来源：http://adc.vehdjk.com

#define X_H
来源：http://sfz.wangdashe.top

#endif
来源：http://ezm.yueranfly.top

[S31] C++：Hello World
来源：http://hqb.aibaodan.cn

#include <iostream>
来源：http://ozs.birdmap.top

int main() { std::cout << "Hello\n"; }
来源：http://rjt.shanyushiyangkeji.top

[S32] C++：字符串
来源：http://lmp.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://rip.sxryk.cn

[S33] C++：vector 增删
来源：http://ups.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ibv.vqdsnc.cn

[S34] C++：遍历 vector
来源：http://fht.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://ndu.zhengqikj.top

[S35] C++：map
来源：http://afx.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hvl.cheryme.top

[S36] C++：unordered_map
来源：http://lld.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ile.jianghu66.top

[S37] C++：set
来源：http://nzg.havefunace.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mey.shanyushiyangtech.top

[S38] C++：排序
来源：http://ikx.meibo888.top

std::sort(v.begin(), v.end());
来源：http://nso.hywenlv.cn

[S39] C++：自定义比较器排序
来源：http://hqt.aibaodan.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rag.zhixingplan.top

[S40] C++：查找元素
来源：http://fsw.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gbn.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://gie.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jii.hnqzz.top

[S42] C++：继承与虚函数
来源：http://kyp.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://tsv.andypj.xyz

[S43] C++：智能指针
来源：http://rac.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://ijv.cqqwz.cn

[S44] C++：引用传参
来源：http://cnm.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://bwh.smart0.xyz

[S45] C++：lambda
来源：http://elr.jlsjyb.cn

auto add = [](int a, int b) { return a + b; };
来源：http://igh.jqgfzy.top

[S46] C++：函数模板
来源：http://tib.fktsv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ogo.haohaochexian.top

[S47] C++：结构化绑定遍历
来源：http://hrd.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://esw.xingfuxueyuan.xyz

[S48] C++：逐行读文件
来源：http://roq.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://ohy.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://noa.sxryk.cn

[S49] C++：写文件
来源：http://jff.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jxs.yj202588.top

[S50] C++：格式化数字
来源：http://yhg.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://meh.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://lhb.meibo888.top

static_cast<double>(a) / b
来源：http://wcm.jyoumei.cn

[S52] C++：const 与 noexcept
来源：http://oxv.xinyue.icu

int size() const noexcept { return n_; }
来源：http://tyi.yongpay.top

[S53] C++：移动语义
来源：http://pkv.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://kqn.yvedp.cn

[S54] C++：异常处理
来源：http://xyr.hnxiangtu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://voi.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://nks.jiagoushi.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fql.316326.xyz

[S56] C++：optional
来源：http://nbz.snrcjt.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pxk.gotoacloud.top

[S57] C++：编译期常量
来源：http://tlp.sxryk.cn

constexpr int N = 10;
来源：http://omf.sufxvd.cn

[S58] C++：命名空间
来源：http://uty.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://aoh.zhongyouzk.top

[S59] C++：静态断言
来源：http://vsb.zhongyouzk.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kbz.jinyuanbaomall.cn

[S60] C++：遍历并删除元素
来源：http://cmg.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dsk.kuanghao11.cn

================================================================================
来源：http://osj.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ewz.yfazqb.com

================================================================================
来源：http://fha.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://nbu.chenlongwang.top

println("Hello")
来源：http://esm.yuxming.cn

[T02] Kotlin：变量
来源：http://nyy.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eos.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://wfk.xingfuxueyuan.xyz

"值: $b"
来源：http://vfe.ivvv.top

[T04] Kotlin：空安全
来源：http://pbj.bjfxy.top

val n: String? = null;  n?.length
来源：http://rjq.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://kab.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xqf.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://vvp.guowangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zgf.yvedp.cn

[T07] Kotlin：集合过滤
来源：http://aiu.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ugz.yueranfly.top

[T08] Kotlin：数据类
来源：http://pvy.vqdsnc.cn

data class User(val name: String, val age: Int)
来源：http://wzx.shanyushiyangkeji.top


<!-- 参考信息 -->