代发 wailian999

name="${1:-default}"
来源：http://veg.feifeiyinyue.top

[R06] 判断命令是否存在
来源：http://ygo.jinghuilouyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qyd.cashguo.top

[R07] if 判断文件
来源：http://nub.redwolf501.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cba.nanxuanxn.top

[R08] 数值比较
来源：http://gdl.nanxinkj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dty.snrcjt.cn

[R09] 字符串比较
来源：http://ojn.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vvj.nanxuanxn.top

[R10] 正则匹配
来源：http://kiy.hfpthk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ezt.gotoacloud.top

[R11] case 多分支
来源：http://kfc.yj20258888.top

case "$1" in
来源：http://ltl.fanxiaobao.xyz

start) echo "启动" ;;
来源：http://vfd.hysaishi.cn

stop)  echo "停止" ;;
来源：http://ecr.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://drj.tanke756.top

esac
来源：http://euk.gogol.net.cn

[R12] for 遍历文件
来源：http://wiq.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://ouj.hcnkem.com

[R13] for 计数循环
来源：http://hsp.jiagoushi.top

for i in {1..10}; do echo "$i"; done
来源：http://pwd.zhongyouzk.top

[R14] C 风格 for
来源：http://pxi.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fei.cashguo.top

[R15] while 逐行读文件
来源：http://cia.yuxming.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yfw.yuanzhike.top

[R16] until 等待条件
来源：http://vey.xylfe.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vhl.cheryme.top

[R17] 数组定义与取值
来源：http://zgy.jinghuilouyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vap.xuanzx.com

[R18] 遍历数组
来源：http://vvy.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wud.gogol.net.cn

[R19] 数组长度
来源：http://grf.aibaodan.cn

echo "${#arr[@]}"
来源：http://fjb.gotoacloud.top

[R20] 关联数组（字典）
来源：http://ubw.birdmap.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://knv.wangdashe.top

[R21] 字符串长度
来源：http://xmc.fzhhl.top

echo "${#s}"
来源：http://vge.xinyue.icu

[R22] 截取子串
来源：http://fld.tarul.cn

echo "${s:0:5}"
来源：http://zta.52xcode.cn

[R23] 字符串替换
来源：http://qrb.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xqy.zhixingplan.top

[R24] 大小写转换
来源：http://krd.xinyue.icu

echo "${s^^}"; echo "${s,,}"
来源：http://hii.nwbrower.top

[R25] 去后缀 / 去前缀
来源：http://kap.ydzc1.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hrn.jinghuilouyu.cn

[R26] 命令替换
来源：http://pcx.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://ipj.0kj1m.cn

[R27] 算术展开
来源：http://eff.pengpengdd.cyou

echo $((1 + 2 * 3))
来源：http://lwp.316326.xyz

[R28] 浮点运算
来源：http://lbl.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://apa.xuanzx.com

[R29] 定义函数
来源：http://jce.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dix.chenjidiqi.icu

[R30] 函数返回状态码
来源：http://gup.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://kfv.snrcjt.cn

[R31] 局部变量
来源：http://dwy.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://wjg.zhiwuduotai.top

[R32] 参数个数校验
来源：http://eij.cucudq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://evr.yj202588.top

[R33] 捕获错误并提示行号
来源：http://opm.zhongyouzk.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://els.uphjek.com

[R34] 退出时清理
来源：http://lwt.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://okt.ctjpmb.com

[R35] 后台执行并等待
来源：http://idg.dianchejie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cqp.zhiwuduotai.top

[R36] 并发执行多个任务
来源：http://duo.cheryme.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cpv.yueranfly.top

[R37] 把输出赋给变量
来源：http://rep.0kj1m.cn

files=$(ls -1)
来源：http://sus.meibo888.top

[R38] 管道串联
来源：http://uqu.sysykeji.top

cat a.txt | grep -i error | wc -l
来源：http://qsy.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://svo.zdqjudy.top

cmd > out.log 2>&1
来源：http://sdf.xuetiantiany.cn

[R40] 追加写日志
来源：http://zfe.gzhubu.top

echo "log" >> out.log
来源：http://qjn.sysykeji.top

[R41] 丢弃输出
来源：http://rfc.mhx1999.top

cmd >/dev/null 2>&1
来源：http://kjy.meibo888.top

[R42] 输入重定向
来源：http://qgy.jqgufenzy.top

wc -l < a.txt
来源：http://sgv.sufxvd.cn

[R43] 按名字查找文件
来源：http://ubb.ydzc1.top

find . -name "*.log" -type f
来源：http://him.yuanzhike.top

[R44] 按修改时间查找
来源：http://ehp.hysaishi.cn

find . -mtime -7 -type f
来源：http://neo.xuetiantiany.cn

[R45] 批量删除
来源：http://gsn.xylfe.cn

find . -name "*.tmp" -delete
来源：http://zbu.tarul.cn

[R46] 递归替换文件内容
来源：http://zrf.9152youxi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sdb.zhiwuduotai.top

[R47] sed 单行替换
来源：http://uxv.tanke756.top

sed -i 's/foo/bar/g' a.txt
来源：http://ozw.hnxiangtu.top

[R48] awk 取指定列
来源：http://fha.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://sba.316326.xyz

[R49] awk 带条件
来源：http://tze.yangfankeji.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wui.yueranfly.top

[R50] awk 求和
来源：http://agx.jinqigufen.top

awk '{s += $2} END {print s}' a.txt
来源：http://rlp.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://aex.quarkkingdee.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bdn.fzhhl.top

[R52] 统计行数
来源：http://ajf.daria6918.cn

wc -l a.txt
来源：http://fvk.sysykeji.top

[R53] 查看文件头与实时尾
来源：http://pol.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wdp.sysykeji.top

[R54] 比较两个文件
来源：http://uak.sysykeji.top

diff a.txt b.txt
来源：http://kyw.jinqigufen.top

[R55] 压缩与解压
来源：http://jew.shzxlz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hhl.fanxiaobao.xyz

[R56] 远程拷贝
来源：http://ivm.sjlbkw.cn

scp file user@host:/path/
来源：http://xuh.redwolf501.top

[R57] 远程执行命令
来源：http://fzh.hfpthk.cn

ssh user@host 'uptime'
来源：http://mba.fzhhl.top

[R58] 下载文件
来源：http://uby.tianlin.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://apy.shuidangran.top

[R59] 发 POST JSON
来源：http://gma.yuxming.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fom.yuanzhike.top

[R60] 只看 HTTP 状态码
来源：http://bur.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mdc.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://fiy.mhx1999.top

df -h;  du -sh *
来源：http://xvv.0kj1m.cn

[R62] 找最占空间的文件
来源：http://rzs.fehbvm.com

du -ah . | sort -rh | head -10
来源：http://srj.hfpthk.cn

[R63] 内存与进程
来源：http://hqo.cucudq.cn

free -h;  ps aux | grep nginx
来源：http://cic.sweek.top

[R64] 结束进程
来源：http://abk.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://fbm.hesvh.cn

[R65] 查看端口占用
来源：http://fpe.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jqv.yueranfly.top

[R66] 定时任务
来源：http://hzx.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://tnx.sxryk.cn

[R67] 生成随机十六进制串
来源：http://wbn.meibo888.top

openssl rand -hex 16
来源：http://smb.yj20258888.top

[R68] 计算文件校验值
来源：http://xwb.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vpw.hnxiangtu.top

[R69] 生成随机密码
来源：http://abf.epnwcf.com

head -c 16 /dev/urandom | base64
来源：http://ari.jianghu66.top

[R70] 时间戳与互转
来源：http://osk.jqgufenzy.top

date +%s;  date -d @1700000000
来源：http://lfm.yvedp.cn

[R71] 日期格式化
来源：http://gfd.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fjw.ybcxt.top

[R72] 等待端口就绪
来源：http://ppx.wangdashe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://aiq.kuanghao11.cn

[R73] 分割大日志
来源：http://onv.ctjpmb.com

split -l 1000 big.log part_
来源：http://uly.svipenyu.cn

[R74] 批量重命名
来源：http://hnk.c1oappe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zpx.mhx1999.top

[R75] 导出环境变量
来源：http://hfz.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://rld.zhongyouzk.top

[R76] 使用临时文件
来源：http://rtf.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xaf.gotoacloud.top

[R77] 读取用户输入
来源：http://glq.jqgufenzy.top

read -rp "请输入: " ans
来源：http://smf.ivvv.top

[R78] 交互式菜单
来源：http://wsv.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ihw.ybcxt.top

[R79] 解析命令行选项
来源：http://dcw.aibaodan.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nez.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://fhe.mhx1999.top

time ./run.sh
来源：http://pxt.hesvh.cn

================================================================================
来源：http://pxz.sxryk.cn

S. C / C++ 专题
来源：http://ymc.redwolf501.top

================================================================================
来源：http://nzf.cashguo.top

[S01] C：Hello World
来源：http://wgp.daria6918.cn

#include <stdio.h>
来源：http://txt.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qea.xylfe.cn

[S02] C：变量与格式化输出
来源：http://izc.gotoacloud.top

int a = 10; printf("%d\n", a);
来源：http://npv.zhengqikj.top

[S03] C：读入整数
来源：http://rwu.hcnkem.com

int x; scanf("%d", &x);
来源：http://aba.zhaomingkeji.xyz

[S04] C：字符串复制
来源：http://efr.haohaochexian.top

char dst[32]; strcpy(dst, "hi");
来源：http://iky.zhiwuduotai.top

[S05] C：字符串长度
来源：http://kuo.nanxinkj.top

strlen(s)
来源：http://ttb.ybcxt.top

[S06] C：字符串比较
来源：http://wlt.xinyue.icu

strcmp(a, b) == 0
来源：http://pla.nwbrower.top

[S07] C：数组遍历求和
来源：http://ooq.xylfe.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gbd.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://rxp.hongshengwenyu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ntr.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://hxl.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xhx.ydzc1.top

[S10] C：指针与解引用
来源：http://oue.cqqwz.cn

int *p = &a;  *p = 5;
来源：http://jzo.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://gar.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://rwk.zhengqikj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wud.vehdjk.com

fclose(f);
来源：http://zzu.epnwcf.com

[S12] C：写文件
来源：http://bqb.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nxv.yfazqb.com

[S13] C：宏定义
来源：http://lvp.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://utu.yueranfly.top

[S14] C：枚举
来源：http://jyj.yuxming.cn

enum Color { RED, GREEN, BLUE };
来源：http://jdp.meibo888.top

[S15] C：类型转换
来源：http://ttl.meibo888.top

(double) a / b
来源：http://bqi.nanxuanxn.top

[S16] C：位操作置位
来源：http://pjf.cqqwz.cn

x |= (1 << 3);
来源：http://esm.bbcook.cn

[S17] C：安全拼接字符串
来源：http://jgq.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://trw.vehdjk.com

[S18] C：命令行参数
来源：http://lik.cashguo.top

int main(int argc, char **argv)
来源：http://icy.fengsongda.top

[S19] C：快速排序
来源：http://upi.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mha.tian-w.cn

[S20] C：二分查找
来源：http://erd.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vwq.sjlbkw.cn

[S21] C：字符类别判断
来源：http://ogz.sufxvd.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tqd.jqgfzy.top

[S22] C：字符串转数字
来源：http://ggr.snrcjt.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jmy.ehwqpu.com

[S23] C：随机数
来源：http://meb.jinqigufen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mks.zdqjudy.top

[S24] C：获取本地时间
来源：http://efh.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pdt.zycfv.cn

[S25] C：内存拷贝
来源：http://sdd.birdmap.top

memcpy(dst, src, n);
来源：http://xzy.9152youxi.cn

[S26] C：内存清零
来源：http://nqv.zhijiandao.cn

memset(a, 0, sizeof a);
来源：http://vwr.nwbrower.top

[S27] C：定义常量
来源：http://qie.epnwcf.com

const double PI = 3.14159;
来源：http://oqp.cdnleiting.top

[S28] C：静态变量
来源：http://jee.jiagoushi.top

static int counter = 0;
来源：http://yjj.xinyue.icu

[S29] C：变参函数
来源：http://kaj.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ysg.ydzc1.top

[S30] C：头文件保护
来源：http://zea.jinqigfzy.top

#ifndef X_H
来源：http://vsx.birdmap.top

#define X_H
来源：http://pmn.fzhhl.top

#endif
来源：http://jik.ydjk.org.cn

[S31] C++：Hello World
来源：http://xgy.yj202588.top

#include <iostream>
来源：http://auc.ctjpmb.com

int main() { std::cout << "Hello\n"; }
来源：http://mgv.quarkkingdee.top

[S32] C++：字符串
来源：http://cvu.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://hnv.hcnkem.com

[S33] C++：vector 增删
来源：http://htw.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dxo.jianghu66.top

[S34] C++：遍历 vector
来源：http://jpm.birdmap.top

for (auto &x : v) { std::cout << x; }
来源：http://qxi.xingfuxueyuan.xyz

[S35] C++：map
来源：http://uvx.yvedp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://shr.zhongyouzk.top

[S36] C++：unordered_map
来源：http://sdl.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://riz.sxryk.cn

[S37] C++：set
来源：http://taz.feifeiyinyue.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kgd.zhongyouzk.top

[S38] C++：排序
来源：http://pui.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://cah.bjfxy.top

[S39] C++：自定义比较器排序
来源：http://fho.bjfxy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zda.dianchejie.cn

[S40] C++：查找元素
来源：http://lfn.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zio.yvedp.cn

[S41] C++：类与构造函数
来源：http://bgz.zhixingplan.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cts.sxryk.cn

[S42] C++：继承与虚函数
来源：http://mqh.gotoacloud.top

class B : public Base { public: void f() override {} };
来源：http://err.hywenlv.cn

[S43] C++：智能指针
来源：http://hgx.havefunace.top

auto p = std::make_unique<int>(5);
来源：http://mab.smart0.xyz

[S44] C++：引用传参
来源：http://rjc.birdmap.top

void inc(int &x) { ++x; }
来源：http://seh.vqdsnc.cn

[S45] C++：lambda
来源：http://amz.sweek.top

auto add = [](int a, int b) { return a + b; };
来源：http://yad.havefunace.top

[S46] C++：函数模板
来源：http://rui.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hue.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://bdn.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dsu.cheryme.top

[S48] C++：逐行读文件
来源：http://dxr.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vka.fehbvm.com

while (std::getline(in, line)) { }
来源：http://mku.fengsongda.top

[S49] C++：写文件
来源：http://bpf.nwbrower.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ead.dianchejie.cn

[S50] C++：格式化数字
来源：http://cgp.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dxp.shuidangran.top

[S51] C++：显式类型转换
来源：http://dfx.ybcxt.top

static_cast<double>(a) / b
来源：http://kxf.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://ooz.epnwcf.com

int size() const noexcept { return n_; }
来源：http://hoy.fengsongda.top

[S53] C++：移动语义
来源：http://kia.xylfe.cn

std::vector<int> w = std::move(v);
来源：http://ukv.ybcxt.top

[S54] C++：异常处理
来源：http://mbg.52xcode.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xzg.pycfn.com

[S55] C++：结构化绑定
来源：http://tys.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tye.jinyuanbaomall.cn

[S56] C++：optional
来源：http://alu.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qbn.gzhubu.top

[S57] C++：编译期常量
来源：http://zsb.52xcode.cn

constexpr int N = 10;
来源：http://ulc.hywenlv.cn

[S58] C++：命名空间
来源：http://nwj.jyoumei.cn

namespace ns { int f() { return 1; } }
来源：http://jcp.gaohongyu789.top

[S59] C++：静态断言
来源：http://puz.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mgc.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://qyu.yfazqb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pvm.tianlin.xyz

================================================================================
来源：http://nbs.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wqs.fzhhl.top

================================================================================
来源：http://xhe.birdmap.top

[T01] Kotlin：Hello World
来源：http://fhk.9152youxi.cn

println("Hello")
来源：http://bpj.jiagoushi.top

[T02] Kotlin：变量
来源：http://ydi.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hpk.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://sny.shuidangran.top

"值: $b"
来源：http://sbz.yueranfly.top

[T04] Kotlin：空安全
来源：http://occ.cheryme.top

val n: String? = null;  n?.length
来源：http://wcy.tianlin.xyz

[T05] Kotlin：when 表达式
来源：http://kzu.tian-w.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ssh.yueranfly.top

[T06] Kotlin：集合映射
来源：http://qho.jyoumei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://asa.nanxinkj.top


<!-- 参考信息 -->