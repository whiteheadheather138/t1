代发 wailian999

readonly PI=3.14
来源：http://lwr.ydzc1.top

[R04] 位置参数
来源：http://muw.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mcc.zhixingplan.top

[R05] 参数默认值
来源：http://iao.hfpthk.cn

name="${1:-default}"
来源：http://znv.fzhhl.top

[R06] 判断命令是否存在
来源：http://lls.shanyushiyangtech.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://afi.shuidangran.top

[R07] if 判断文件
来源：http://pac.shanyushiyangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oet.nanxinkj.top

[R08] 数值比较
来源：http://kdf.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kjd.0kj1m.cn

[R09] 字符串比较
来源：http://vxp.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eio.tanke756.top

[R10] 正则匹配
来源：http://hdq.hfpthk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cfv.hnxiangtu.top

[R11] case 多分支
来源：http://gsm.gotoacloud.top

case "$1" in
来源：http://kdw.ehwqpu.com

start) echo "启动" ;;
来源：http://rer.ybcxt.top

stop)  echo "停止" ;;
来源：http://cii.uphjek.com

*)     echo "未知命令" ;;
来源：http://yqa.52xcode.cn

esac
来源：http://ezs.sxryk.cn

[R12] for 遍历文件
来源：http://mth.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://bmc.birdmap.top

[R13] for 计数循环
来源：http://vvr.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://izp.aibaodan.cn

[R14] C 风格 for
来源：http://yty.iojbl.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://due.zdqjudy.top

[R15] while 逐行读文件
来源：http://mnn.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tum.cashguo.top

[R16] until 等待条件
来源：http://lwc.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ugp.ppjwa.cn

[R17] 数组定义与取值
来源：http://psy.ywan-chungtsiang.top

arr=(a b c); echo "${arr[0]}"
来源：http://dwp.shangyingyoupin.top

[R18] 遍历数组
来源：http://wdg.aizwys.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://new.ydjk.org.cn

[R19] 数组长度
来源：http://wij.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://eou.nwbrower.top

[R20] 关联数组（字典）
来源：http://vpu.iojbl.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hkt.xziqi.cn

[R21] 字符串长度
来源：http://nhs.ctjpmb.com

echo "${#s}"
来源：http://chu.aizwys.cn

[R22] 截取子串
来源：http://gwv.sxryk.cn

echo "${s:0:5}"
来源：http://yms.zhengqikj.top

[R23] 字符串替换
来源：http://qpw.kuanghao11.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hmi.gzhubu.top

[R24] 大小写转换
来源：http://rrb.ydjk.org.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ihy.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://lax.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ojc.yonumen.top

[R26] 命令替换
来源：http://agc.sysykeji.top

now=$(date +%F); echo "$now"
来源：http://xvl.snrcjt.cn

[R27] 算术展开
来源：http://qbp.yvedp.cn

echo $((1 + 2 * 3))
来源：http://ztq.zhengqikj.top

[R28] 浮点运算
来源：http://nvh.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://fct.gaohongyu789.top

[R29] 定义函数
来源：http://anv.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://teo.xinyue.icu

[R30] 函数返回状态码
来源：http://ioz.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://ykv.yuanzhike.top

[R31] 局部变量
来源：http://jjq.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://izl.hcnkem.com

[R32] 参数个数校验
来源：http://zzs.hnqzz.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iew.pycfn.com

[R33] 捕获错误并提示行号
来源：http://rnu.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aac.sxryk.cn

[R34] 退出时清理
来源：http://hoq.bbcook.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tik.zhongyouzk.top

[R35] 后台执行并等待
来源：http://din.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zps.wangdashe.top

[R36] 并发执行多个任务
来源：http://gfs.zhengqikj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pbw.ybcxt.top

[R37] 把输出赋给变量
来源：http://qus.yangfankeji.com

files=$(ls -1)
来源：http://jdq.uphjek.com

[R38] 管道串联
来源：http://rim.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://mme.gotoacloud.top

[R39] 重定向标准输出与错误
来源：http://cjp.kuanghao11.cn

cmd > out.log 2>&1
来源：http://rey.havefunace.top

[R40] 追加写日志
来源：http://jdm.shanyushiyangkeji.top

echo "log" >> out.log
来源：http://zhj.gzhubu.top

[R41] 丢弃输出
来源：http://cpk.andypj.xyz

cmd >/dev/null 2>&1
来源：http://iwr.snrcjt.cn

[R42] 输入重定向
来源：http://eub.gotoacloud.top

wc -l < a.txt
来源：http://ukg.zdbjq.cn

[R43] 按名字查找文件
来源：http://aym.gaohongyu789.top

find . -name "*.log" -type f
来源：http://vtk.yueranfly.top

[R44] 按修改时间查找
来源：http://rqx.snrcjt.cn

find . -mtime -7 -type f
来源：http://nsk.kuanghao11.cn

[R45] 批量删除
来源：http://yfz.cashguo.top

find . -name "*.tmp" -delete
来源：http://nau.daria6918.cn

[R46] 递归替换文件内容
来源：http://yfj.gzhubu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tys.shangyingyoupin.top

[R47] sed 单行替换
来源：http://rcb.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://gwe.ppjwa.cn

[R48] awk 取指定列
来源：http://hxf.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://tye.cucudq.cn

[R49] awk 带条件
来源：http://ese.ehwqpu.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hby.gaohongyu789.top

[R50] awk 求和
来源：http://pvi.52xcode.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zhv.ppjwa.cn

[R51] 排序去重取前几
来源：http://duj.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hsy.fehbvm.com

[R52] 统计行数
来源：http://bwr.zdbjq.cn

wc -l a.txt
来源：http://few.cheryme.top

[R53] 查看文件头与实时尾
来源：http://cth.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dda.zdbjq.cn

[R54] 比较两个文件
来源：http://khi.cucudq.cn

diff a.txt b.txt
来源：http://weo.zhengqikj.top

[R55] 压缩与解压
来源：http://lsa.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nbc.jinghuilouyu.cn

[R56] 远程拷贝
来源：http://yjb.yueranfly.top

scp file user@host:/path/
来源：http://wdj.svipenyu.cn

[R57] 远程执行命令
来源：http://wsl.daria6918.cn

ssh user@host 'uptime'
来源：http://wfa.quarkkingdee.top

[R58] 下载文件
来源：http://val.ivvv.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rye.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://lpe.jiagoushi.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kzo.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://hqy.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iyw.zhixingplan.top

[R61] 磁盘占用
来源：http://whn.pycfn.com

df -h;  du -sh *
来源：http://vds.shanyushiyangtech.top

[R62] 找最占空间的文件
来源：http://ufu.aizwys.cn

du -ah . | sort -rh | head -10
来源：http://vxk.cashguo.top

[R63] 内存与进程
来源：http://vfd.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://nod.shuidangran.top

[R64] 结束进程
来源：http://wcd.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://xst.yj20258888.top

[R65] 查看端口占用
来源：http://eyn.ivvv.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://maz.yueranfly.top

[R66] 定时任务
来源：http://lln.zhongyouzk.top

crontab -e;  crontab -l
来源：http://bks.zdqjudy.top

[R67] 生成随机十六进制串
来源：http://ruj.vehdjk.com

openssl rand -hex 16
来源：http://ifo.xylfe.cn

[R68] 计算文件校验值
来源：http://itj.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xxp.52xcode.cn

[R69] 生成随机密码
来源：http://gfi.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://fxr.yvedp.cn

[R70] 时间戳与互转
来源：http://rkn.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://oxx.yonumen.top

[R71] 日期格式化
来源：http://ttw.jlsjyb.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uhx.smart0.xyz

[R72] 等待端口就绪
来源：http://kal.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jza.9152youxi.cn

[R73] 分割大日志
来源：http://evd.hysaishi.cn

split -l 1000 big.log part_
来源：http://clg.9152youxi.cn

[R74] 批量重命名
来源：http://guc.xziqi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oeg.yueranfly.top

[R75] 导出环境变量
来源：http://iwv.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://imh.fktsv.cn

[R76] 使用临时文件
来源：http://pgk.guowangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oro.pengpengdd.cyou

[R77] 读取用户输入
来源：http://nzh.zhaomingkeji.xyz

read -rp "请输入: " ans
来源：http://gih.52xcode.cn

[R78] 交互式菜单
来源：http://uxn.mhx1999.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tej.yuxming.cn

[R79] 解析命令行选项
来源：http://pjv.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ysg.316326.xyz

[R80] 查看脚本执行耗时
来源：http://ykw.ybcxt.top

time ./run.sh
来源：http://bos.dianchejie.cn

================================================================================
来源：http://fes.chenzaomai.com

S. C / C++ 专题
来源：http://lsx.jlsjyb.cn

================================================================================
来源：http://kqt.fktsv.cn

[S01] C：Hello World
来源：http://zyx.0kj1m.cn

#include <stdio.h>
来源：http://ghh.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ser.cheryme.top

[S02] C：变量与格式化输出
来源：http://kqu.hesvh.cn

int a = 10; printf("%d\n", a);
来源：http://sdy.havefunace.top

[S03] C：读入整数
来源：http://yul.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://etk.nanxuanxn.top

[S04] C：字符串复制
来源：http://hqh.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://fiw.hesvh.cn

[S05] C：字符串长度
来源：http://yvi.zhijiandao.cn

strlen(s)
来源：http://qfg.iojbl.cn

[S06] C：字符串比较
来源：http://bgu.fktsv.cn

strcmp(a, b) == 0
来源：http://wof.ctjpmb.com

[S07] C：数组遍历求和
来源：http://tvl.nanxinkj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://svv.mhx1999.top

[S08] C：动态内存分配与释放
来源：http://etz.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rjh.aibaodan.cn

[S09] C：结构体定义与初始化
来源：http://num.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lfj.jinqigfzy.top

[S10] C：指针与解引用
来源：http://mhz.tian-w.cn

int *p = &a;  *p = 5;
来源：http://sye.hnxiangtu.top

[S11] C：逐行读文件
来源：http://irg.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://civ.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://diw.jinqigufen.top

fclose(f);
来源：http://mdl.tianlin.xyz

[S12] C：写文件
来源：http://odi.yueranfly.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yuo.xingfuxueyuan.xyz

[S13] C：宏定义
来源：http://rtg.daxiang520.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xfd.zycfv.cn

[S14] C：枚举
来源：http://sfa.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://etk.zhixingplan.top

[S15] C：类型转换
来源：http://ngm.pengpengdd.cyou

(double) a / b
来源：http://tux.mhx1999.top

[S16] C：位操作置位
来源：http://xga.ydjk.org.cn

x |= (1 << 3);
来源：http://fho.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://uxr.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oms.cheryme.top

[S18] C：命令行参数
来源：http://pot.ydjk.org.cn

int main(int argc, char **argv)
来源：http://mls.wangdashe.top

[S19] C：快速排序
来源：http://ljt.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://crj.gotoacloud.top

[S20] C：二分查找
来源：http://jma.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://efr.hesvh.cn

[S21] C：字符类别判断
来源：http://ejt.c1oappe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ztq.xinyue.icu

[S22] C：字符串转数字
来源：http://qvs.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://wzp.iojbl.cn

[S23] C：随机数
来源：http://njl.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vah.gaohongyu789.top

[S24] C：获取本地时间
来源：http://kdd.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://izv.ehwqpu.com

[S25] C：内存拷贝
来源：http://wuz.hfpthk.cn

memcpy(dst, src, n);
来源：http://ovl.tian-w.cn

[S26] C：内存清零
来源：http://wlw.yonumen.top

memset(a, 0, sizeof a);
来源：http://xpv.ybcxt.top

[S27] C：定义常量
来源：http://oed.c1oappe.top

const double PI = 3.14159;
来源：http://nwe.cucudq.cn

[S28] C：静态变量
来源：http://wwy.xuanzx.com

static int counter = 0;
来源：http://zwz.zhijiandao.cn

[S29] C：变参函数
来源：http://tnn.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://skg.ydjk.org.cn

[S30] C：头文件保护
来源：http://ego.ybcxt.top

#ifndef X_H
来源：http://hvh.yj20258.top

#define X_H
来源：http://pll.yanxiufei.cn

#endif
来源：http://dlh.hesvh.cn

[S31] C++：Hello World
来源：http://bcq.jqgfzy.top

#include <iostream>
来源：http://fto.zhengqikj.top

int main() { std::cout << "Hello\n"; }
来源：http://lgv.xziqi.cn

[S32] C++：字符串
来源：http://gqh.sufxvd.cn

std::string s = "hi";  s += "!";
来源：http://kss.aizwys.cn

[S33] C++：vector 增删
来源：http://kfp.yanxiufei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dnx.chenzaomai.com

[S34] C++：遍历 vector
来源：http://vfi.cheryme.top

for (auto &x : v) { std::cout << x; }
来源：http://vhc.hcnkem.com

[S35] C++：map
来源：http://dlz.cheryme.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kzg.chenlongwang.top

[S36] C++：unordered_map
来源：http://thw.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dwh.xziqi.cn

[S37] C++：set
来源：http://hvp.wangshuangyany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wrv.dianchejie.cn

[S38] C++：排序
来源：http://bcm.yj202588.top

std::sort(v.begin(), v.end());
来源：http://zui.nanxinkj.top

[S39] C++：自定义比较器排序
来源：http://swr.fehbvm.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oap.sxryk.cn

[S40] C++：查找元素
来源：http://qjd.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gji.hfpthk.cn

[S41] C++：类与构造函数
来源：http://ldn.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mqm.nanxuanxn.top

[S42] C++：继承与虚函数
来源：http://oac.cqqwz.cn

class B : public Base { public: void f() override {} };
来源：http://inl.kuanghao11.cn

[S43] C++：智能指针
来源：http://ldn.nanxuanxn.top

auto p = std::make_unique<int>(5);
来源：http://she.zhaomingkeji.xyz

[S44] C++：引用传参
来源：http://zvl.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://dju.sweek.top

[S45] C++：lambda
来源：http://lfc.dianchejie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vxz.chenzaomai.com

[S46] C++：函数模板
来源：http://ewn.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://edb.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://vum.ywan-chungtsiang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vqa.9152youxi.cn

[S48] C++：逐行读文件
来源：http://dza.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://klq.jinqigufen.top

while (std::getline(in, line)) { }
来源：http://aoz.fzhhl.top

[S49] C++：写文件
来源：http://jvz.hfpthk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://klm.andypj.xyz

[S50] C++：格式化数字
来源：http://ozf.svipenyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iic.meibo888.top

[S51] C++：显式类型转换
来源：http://obj.daria6918.cn

static_cast<double>(a) / b
来源：http://qnm.meibo888.top

[S52] C++：const 与 noexcept
来源：http://jjj.jyoumei.cn

int size() const noexcept { return n_; }
来源：http://vjq.yvedp.cn

[S53] C++：移动语义
来源：http://qlj.tianlin.xyz

std::vector<int> w = std::move(v);
来源：http://usp.0kj1m.cn

[S54] C++：异常处理
来源：http://nge.birdmap.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gwo.zhoulong.xyz

[S55] C++：结构化绑定
来源：http://xre.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://qxh.jyoumei.cn

[S56] C++：optional
来源：http://vtr.dianchejie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cif.vehdjk.com

[S57] C++：编译期常量
来源：http://oiw.cdnleiting.top

constexpr int N = 10;
来源：http://aau.meibo888.top

[S58] C++：命名空间
来源：http://irj.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://kui.ctjpmb.com

[S59] C++：静态断言
来源：http://ycr.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lhd.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://glb.yanxiufei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cue.cashguo.top

================================================================================
来源：http://qap.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mpu.sjlbkw.cn

================================================================================
来源：http://wkx.bjfxy.top

[T01] Kotlin：Hello World
来源：http://rtb.yuxming.cn

println("Hello")
来源：http://tln.daxiang520.top

[T02] Kotlin：变量
来源：http://ooq.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kmc.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://yij.shanyushiyangkeji.top

"值: $b"
来源：http://rqx.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://sam.hnqzz.top

val n: String? = null;  n?.length
来源：http://gph.fehbvm.com


<!-- 参考信息 -->