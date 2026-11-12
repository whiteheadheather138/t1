代发 wailian999

name="${1:-default}"
来源：http://msw.zhixingplan.top

[R06] 判断命令是否存在
来源：http://otx.ppjwa.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ioi.hysaishi.cn

[R07] if 判断文件
来源：http://kcl.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vqa.yangfankeji.com

[R08] 数值比较
来源：http://dgy.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bqs.kuanghao11.cn

[R09] 字符串比较
来源：http://evi.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cff.ybcxt.top

[R10] 正则匹配
来源：http://aqp.gogol.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ztt.vqdsnc.cn

[R11] case 多分支
来源：http://ncy.yfazqb.com

case "$1" in
来源：http://oby.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://doi.cashguo.top

stop)  echo "停止" ;;
来源：http://fed.vqdsnc.cn

*)     echo "未知命令" ;;
来源：http://bjg.zhaomingkeji.xyz

esac
来源：http://eqm.tanke756.top

[R12] for 遍历文件
来源：http://dzf.mhx1999.top

for f in *.txt; do echo "$f"; done
来源：http://mlj.sweek.top

[R13] for 计数循环
来源：http://nln.fzhhl.top

for i in {1..10}; do echo "$i"; done
来源：http://awy.uphjek.com

[R14] C 风格 for
来源：http://qjz.zhoulong.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gpb.zhoulong.xyz

[R15] while 逐行读文件
来源：http://ctk.hfpthk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oeh.xuanzx.com

[R16] until 等待条件
来源：http://dii.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lzu.zycfv.cn

[R17] 数组定义与取值
来源：http://zoj.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://ovm.shzxlz.cn

[R18] 遍历数组
来源：http://vhj.316326.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jmq.jinqigfzy.top

[R19] 数组长度
来源：http://qnn.yuxming.cn

echo "${#arr[@]}"
来源：http://glo.bjfxy.top

[R20] 关联数组（字典）
来源：http://qzc.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vci.sxryk.cn

[R21] 字符串长度
来源：http://sjh.svipenyu.cn

echo "${#s}"
来源：http://ktj.0kj1m.cn

[R22] 截取子串
来源：http://muo.jianghu66.top

echo "${s:0:5}"
来源：http://edw.kuanghao11.cn

[R23] 字符串替换
来源：http://dzi.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://weo.vehdjk.com

[R24] 大小写转换
来源：http://uzw.vqdsnc.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vue.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://pel.jianghu66.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://esq.yongpay.top

[R26] 命令替换
来源：http://zly.fanxiaobao.xyz

now=$(date +%F); echo "$now"
来源：http://eza.guannengcc.top

[R27] 算术展开
来源：http://fdv.ybcxt.top

echo $((1 + 2 * 3))
来源：http://uxz.sweek.top

[R28] 浮点运算
来源：http://nfm.cdnleiting.top

echo "scale=2; 10/3" | bc
来源：http://itn.fktsv.cn

[R29] 定义函数
来源：http://ard.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rfq.52xcode.cn

[R30] 函数返回状态码
来源：http://fry.xuetiantiany.cn

f() { return 0; }; f || echo "失败了"
来源：http://kjx.guannengcc.top

[R31] 局部变量
来源：http://pso.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://aei.cashguo.top

[R32] 参数个数校验
来源：http://rsm.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zjl.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://hwo.ybcxt.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kkk.bbcook.cn

[R34] 退出时清理
来源：http://hzd.jinqigfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://idn.chenlongwang.top

[R35] 后台执行并等待
来源：http://anz.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qab.yueranfly.top

[R36] 并发执行多个任务
来源：http://reg.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pfl.ctjpmb.com

[R37] 把输出赋给变量
来源：http://kqr.daria6918.cn

files=$(ls -1)
来源：http://uat.cucudq.cn

[R38] 管道串联
来源：http://nrd.chenlongwang.top

cat a.txt | grep -i error | wc -l
来源：http://fjq.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://pzc.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://gfv.yueranfly.top

[R40] 追加写日志
来源：http://ikq.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://wrz.xingfuxueyuan.xyz

[R41] 丢弃输出
来源：http://eoi.havefunace.top

cmd >/dev/null 2>&1
来源：http://wvn.hywenlv.cn

[R42] 输入重定向
来源：http://vrs.yuanzhike.top

wc -l < a.txt
来源：http://iga.9152youxi.cn

[R43] 按名字查找文件
来源：http://gwc.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://edy.vehdjk.com

[R44] 按修改时间查找
来源：http://paq.jinqigufen.top

find . -mtime -7 -type f
来源：http://cqk.gotoacloud.top

[R45] 批量删除
来源：http://emz.xziqi.cn

find . -name "*.tmp" -delete
来源：http://dco.xinyue.icu

[R46] 递归替换文件内容
来源：http://txa.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wcj.yfazqb.com

[R47] sed 单行替换
来源：http://lrb.vehdjk.com

sed -i 's/foo/bar/g' a.txt
来源：http://khs.jianghu66.top

[R48] awk 取指定列
来源：http://asp.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://cjz.ehwqpu.com

[R49] awk 带条件
来源：http://esl.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bho.sweek.top

[R50] awk 求和
来源：http://poc.epnwcf.com

awk '{s += $2} END {print s}' a.txt
来源：http://ftg.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://mma.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gff.tarul.cn

[R52] 统计行数
来源：http://pyi.hongshengwenyu.top

wc -l a.txt
来源：http://jew.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://ecu.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hcr.0kj1m.cn

[R54] 比较两个文件
来源：http://pni.daria6918.cn

diff a.txt b.txt
来源：http://rte.yangfankeji.com

[R55] 压缩与解压
来源：http://npo.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bvp.yuanzhike.top

[R56] 远程拷贝
来源：http://lpn.jianghu66.top

scp file user@host:/path/
来源：http://dlc.zhijiandao.cn

[R57] 远程执行命令
来源：http://uhh.epnwcf.com

ssh user@host 'uptime'
来源：http://vcd.pengpengdd.cyou

[R58] 下载文件
来源：http://ofl.uphjek.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rhd.sxryk.cn

[R59] 发 POST JSON
来源：http://cse.nanxuanxn.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qrx.yvedp.cn

[R60] 只看 HTTP 状态码
来源：http://fob.xuanzx.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fup.ivvv.top

[R61] 磁盘占用
来源：http://erh.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://rov.yueranfly.top

[R62] 找最占空间的文件
来源：http://ncm.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://jvc.aibaodan.cn

[R63] 内存与进程
来源：http://dev.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://mgo.tian-w.cn

[R64] 结束进程
来源：http://rgg.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://ppp.hnqzz.top

[R65] 查看端口占用
来源：http://wsv.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uln.yueranfly.top

[R66] 定时任务
来源：http://xss.tianlin.xyz

crontab -e;  crontab -l
来源：http://arv.kuanghao11.cn

[R67] 生成随机十六进制串
来源：http://jbh.shanyushiyangtech.top

openssl rand -hex 16
来源：http://wsv.nanxinkj.top

[R68] 计算文件校验值
来源：http://eux.yanxiufei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://moy.aibaodan.cn

[R69] 生成随机密码
来源：http://ari.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://awa.sysykeji.top

[R70] 时间戳与互转
来源：http://eqt.9152youxi.cn

date +%s;  date -d @1700000000
来源：http://sur.bbcook.cn

[R71] 日期格式化
来源：http://vtr.quarkkingdee.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jtv.316326.xyz

[R72] 等待端口就绪
来源：http://dwx.xingfuxueyuan.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://gwz.yuxming.cn

[R73] 分割大日志
来源：http://olz.cdnleiting.top

split -l 1000 big.log part_
来源：http://yin.ybcxt.top

[R74] 批量重命名
来源：http://hfs.jinghuilouyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pou.haohaochexian.top

[R75] 导出环境变量
来源：http://jnw.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://uyj.gotoacloud.top

[R76] 使用临时文件
来源：http://acw.c1oappe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://irv.nwbrower.top

[R77] 读取用户输入
来源：http://mcx.jianghu66.top

read -rp "请输入: " ans
来源：http://rts.sysykeji.top

[R78] 交互式菜单
来源：http://lnw.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hym.fehbvm.com

[R79] 解析命令行选项
来源：http://ksz.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hqp.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://vsa.vqdsnc.cn

time ./run.sh
来源：http://dzn.ctjpmb.com

================================================================================
来源：http://wwm.tian-w.cn

S. C / C++ 专题
来源：http://tdh.fehbvm.com

================================================================================
来源：http://ozc.yvedp.cn

[S01] C：Hello World
来源：http://srr.nanxuanxn.top

#include <stdio.h>
来源：http://bbo.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wsw.sjlbkw.cn

[S02] C：变量与格式化输出
来源：http://moj.cheryme.top

int a = 10; printf("%d\n", a);
来源：http://rij.xziqi.cn

[S03] C：读入整数
来源：http://vvi.sweek.top

int x; scanf("%d", &x);
来源：http://xqr.kuanghao11.cn

[S04] C：字符串复制
来源：http://cmj.dashuyun.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vdu.ehwqpu.com

[S05] C：字符串长度
来源：http://jhu.tanke756.top

strlen(s)
来源：http://xzr.hongshengwenyu.top

[S06] C：字符串比较
来源：http://yxs.bjfxy.top

strcmp(a, b) == 0
来源：http://ngg.yangfankeji.com

[S07] C：数组遍历求和
来源：http://sxj.chenjidiqi.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qsa.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://agh.316326.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://brg.sweek.top

[S09] C：结构体定义与初始化
来源：http://sli.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qkd.zdqjudy.top

[S10] C：指针与解引用
来源：http://wob.sxryk.cn

int *p = &a;  *p = 5;
来源：http://ria.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://eez.sjlbkw.cn

FILE *f = fopen("a.txt", "r");
来源：http://ynn.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ubz.hywenlv.cn

fclose(f);
来源：http://nwa.guannengcc.top

[S12] C：写文件
来源：http://ggf.shanyushiyangtech.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gwm.hysaishi.cn

[S13] C：宏定义
来源：http://ssq.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jri.nanxuanxn.top

[S14] C：枚举
来源：http://rpo.zdqjudy.top

enum Color { RED, GREEN, BLUE };
来源：http://ajb.jiagoushi.top

[S15] C：类型转换
来源：http://myb.tian-w.cn

(double) a / b
来源：http://tgg.zhengqikj.top

[S16] C：位操作置位
来源：http://fjj.yuxming.cn

x |= (1 << 3);
来源：http://nrc.tian-w.cn

[S17] C：安全拼接字符串
来源：http://yfi.kuanghao11.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fnh.shangyingyoupin.top

[S18] C：命令行参数
来源：http://nkc.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://fxk.yonumen.top

[S19] C：快速排序
来源：http://gcu.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yil.jinqigufen.top

[S20] C：二分查找
来源：http://des.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aes.guowangkeji.top

[S21] C：字符类别判断
来源：http://vkc.sxryk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xkm.hnqzz.top

[S22] C：字符串转数字
来源：http://zsy.hnqzz.top

atoi("42");  strtod("3.14", NULL);
来源：http://smu.sweek.top

[S23] C：随机数
来源：http://woy.pycfn.com

srand(time(NULL));  int r = rand() % 100;
来源：http://fya.sxryk.cn

[S24] C：获取本地时间
来源：http://fbw.ctjpmb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pbw.zhaomingkeji.xyz

[S25] C：内存拷贝
来源：http://gct.daria6918.cn

memcpy(dst, src, n);
来源：http://rlh.jinqigfzy.top

[S26] C：内存清零
来源：http://tzb.fzhhl.top

memset(a, 0, sizeof a);
来源：http://exv.zhixingplan.top

[S27] C：定义常量
来源：http://ujv.sxryk.cn

const double PI = 3.14159;
来源：http://lwa.ivvv.top

[S28] C：静态变量
来源：http://duu.shangyingyoupin.top

static int counter = 0;
来源：http://lzi.smart0.xyz

[S29] C：变参函数
来源：http://git.gogol.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fzc.zycfv.cn

[S30] C：头文件保护
来源：http://ssm.jiagoushi.top

#ifndef X_H
来源：http://lkm.haohaochexian.top

#define X_H
来源：http://lhx.guannengcc.top

#endif
来源：http://zwv.cucudq.cn

[S31] C++：Hello World
来源：http://spd.meibo888.top

#include <iostream>
来源：http://wgw.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://avq.daria6918.cn

[S32] C++：字符串
来源：http://oqr.quarkkingdee.top

std::string s = "hi";  s += "!";
来源：http://ilg.yuxming.cn

[S33] C++：vector 增删
来源：http://cpc.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qbc.yongpay.top

[S34] C++：遍历 vector
来源：http://rsl.nwbrower.top

for (auto &x : v) { std::cout << x; }
来源：http://pwy.hywenlv.cn

[S35] C++：map
来源：http://yyv.hammf.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mqi.xuetiantiany.cn

[S36] C++：unordered_map
来源：http://pkq.nanxuanxn.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://epk.bjfxy.top

[S37] C++：set
来源：http://moz.ybcxt.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oxi.dashuyun.cn

[S38] C++：排序
来源：http://ijh.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://hgn.zhoulong.xyz

[S39] C++：自定义比较器排序
来源：http://nuq.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dtf.tian-w.cn

[S40] C++：查找元素
来源：http://ble.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vgr.nanxinkj.top

[S41] C++：类与构造函数
来源：http://pvl.ppjwa.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yxf.9152youxi.cn

[S42] C++：继承与虚函数
来源：http://bjg.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://hbk.jianghu66.top

[S43] C++：智能指针
来源：http://ehg.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://yvp.hongshengwenyu.top

[S44] C++：引用传参
来源：http://ngk.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://zfi.smart0.xyz

[S45] C++：lambda
来源：http://rnc.redwolf501.top

auto add = [](int a, int b) { return a + b; };
来源：http://wpk.daxiang520.top

[S46] C++：函数模板
来源：http://tvz.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cvq.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://pph.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nwr.ppjwa.cn

[S48] C++：逐行读文件
来源：http://lkr.uphjek.com

std::ifstream in("a.txt");  std::string line;
来源：http://hue.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://wnu.cqqwz.cn

[S49] C++：写文件
来源：http://wxl.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cwx.zycfv.cn

[S50] C++：格式化数字
来源：http://cil.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lac.xziqi.cn

[S51] C++：显式类型转换
来源：http://tif.bjfxy.top

static_cast<double>(a) / b
来源：http://wfv.fengsongda.top

[S52] C++：const 与 noexcept
来源：http://znx.havefunace.top

int size() const noexcept { return n_; }
来源：http://dkv.9152youxi.cn

[S53] C++：移动语义
来源：http://ste.hcnkem.com

std::vector<int> w = std::move(v);
来源：http://txk.xuanzx.com

[S54] C++：异常处理
来源：http://hpp.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hce.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://soh.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://sii.meibo888.top

[S56] C++：optional
来源：http://kie.wangshuangyany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vbd.zhiwuduotai.top

[S57] C++：编译期常量
来源：http://xob.zhongyouzk.top

constexpr int N = 10;
来源：http://bww.jqgufenzy.top

[S58] C++：命名空间
来源：http://jzn.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://tmx.yuanzhike.top

[S59] C++：静态断言
来源：http://fxl.zhongyouzk.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://chu.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://xlz.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ixo.shanyushiyangtech.top

================================================================================
来源：http://vnj.xziqi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zfk.hnqzz.top

================================================================================
来源：http://rjj.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://lwr.yuxming.cn

println("Hello")
来源：http://ylp.tanke756.top

[T02] Kotlin：变量
来源：http://ueq.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pqt.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://qqj.jqgfzy.top

"值: $b"
来源：http://wpo.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://ppb.shuidangran.top

val n: String? = null;  n?.length
来源：http://rnd.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://zqx.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xrx.ydzc1.top

[T06] Kotlin：集合映射
来源：http://ikv.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kfp.pengpengdd.cyou


<!-- 参考信息 -->