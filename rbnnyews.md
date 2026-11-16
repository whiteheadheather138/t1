代发 wailian999

readonly PI=3.14
来源：http://ocp.xuetiantiany.cn

[R04] 位置参数
来源：http://vkh.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://igh.hongshengwenyu.top

[R05] 参数默认值
来源：http://mfl.aibaodan.cn

name="${1:-default}"
来源：http://mgt.cucudq.cn

[R06] 判断命令是否存在
来源：http://trb.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wxl.hnxiangtu.top

[R07] if 判断文件
来源：http://udo.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://box.jinghuilouyu.cn

[R08] 数值比较
来源：http://wad.redwolf501.top

if (( a > b )); then echo "a 更大"; fi
来源：http://opv.nwbrower.top

[R09] 字符串比较
来源：http://abf.316326.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aor.zhaomingkeji.xyz

[R10] 正则匹配
来源：http://aic.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pyj.birdmap.top

[R11] case 多分支
来源：http://vsv.shanyushiyangkeji.top

case "$1" in
来源：http://vnx.jiagoushi.top

start) echo "启动" ;;
来源：http://eon.hfpthk.cn

stop)  echo "停止" ;;
来源：http://jme.tian-w.cn

*)     echo "未知命令" ;;
来源：http://avi.yongpay.top

esac
来源：http://ydx.gotoacloud.top

[R12] for 遍历文件
来源：http://tpu.pengpengdd.cyou

for f in *.txt; do echo "$f"; done
来源：http://deb.jyoumei.cn

[R13] for 计数循环
来源：http://bnb.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://pce.pycfn.com

[R14] C 风格 for
来源：http://sdh.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bol.ctjpmb.com

[R15] while 逐行读文件
来源：http://axs.xuetiantiany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ygl.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://usr.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ypr.tianlin.xyz

[R17] 数组定义与取值
来源：http://qwo.ywan-chungtsiang.top

arr=(a b c); echo "${arr[0]}"
来源：http://mvu.sjlbkw.cn

[R18] 遍历数组
来源：http://ubm.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cwz.fzhhl.top

[R19] 数组长度
来源：http://mgl.yuxming.cn

echo "${#arr[@]}"
来源：http://rzh.ydzc1.top

[R20] 关联数组（字典）
来源：http://yzf.dianchejie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hcm.fzhhl.top

[R21] 字符串长度
来源：http://ekk.zdqjudy.top

echo "${#s}"
来源：http://pmd.yonumen.top

[R22] 截取子串
来源：http://mvi.hcnkem.com

echo "${s:0:5}"
来源：http://tpk.yongpay.top

[R23] 字符串替换
来源：http://fag.shuidangran.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gwn.xuetiantiany.cn

[R24] 大小写转换
来源：http://zoq.epnwcf.com

echo "${s^^}"; echo "${s,,}"
来源：http://tdd.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://abq.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://szc.cheryme.top

[R26] 命令替换
来源：http://hgz.yvedp.cn

now=$(date +%F); echo "$now"
来源：http://zuy.nwbrower.top

[R27] 算术展开
来源：http://pvd.havefunace.top

echo $((1 + 2 * 3))
来源：http://jtv.zhixingplan.top

[R28] 浮点运算
来源：http://nhv.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://yse.tarul.cn

[R29] 定义函数
来源：http://sue.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://urd.zhengqikj.top

[R30] 函数返回状态码
来源：http://tbq.redwolf501.top

f() { return 0; }; f || echo "失败了"
来源：http://gfd.ydjk.org.cn

[R31] 局部变量
来源：http://tbv.yongpay.top

f() { local x=1; echo "$x"; }
来源：http://zpb.xziqi.cn

[R32] 参数个数校验
来源：http://jnj.9152youxi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pyr.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://klu.epnwcf.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hxo.sjlbkw.cn

[R34] 退出时清理
来源：http://ivw.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://alg.zycfv.cn

[R35] 后台执行并等待
来源：http://qoz.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vdh.wangshuangyany.cn

[R36] 并发执行多个任务
来源：http://uzl.tianlin.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hlt.hammf.cn

[R37] 把输出赋给变量
来源：http://lvo.hesvh.cn

files=$(ls -1)
来源：http://vzg.gotoacloud.top

[R38] 管道串联
来源：http://udn.jyoumei.cn

cat a.txt | grep -i error | wc -l
来源：http://rss.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://qxn.fktsv.cn

cmd > out.log 2>&1
来源：http://hxf.tian-w.cn

[R40] 追加写日志
来源：http://dcz.tianlin.xyz

echo "log" >> out.log
来源：http://cba.ctjpmb.com

[R41] 丢弃输出
来源：http://bey.nanxinkj.top

cmd >/dev/null 2>&1
来源：http://bfh.gotoacloud.top

[R42] 输入重定向
来源：http://sox.sjlbkw.cn

wc -l < a.txt
来源：http://sou.wangdashe.top

[R43] 按名字查找文件
来源：http://eae.sufxvd.cn

find . -name "*.log" -type f
来源：http://fdr.tarul.cn

[R44] 按修改时间查找
来源：http://mqy.wangshuangyany.cn

find . -mtime -7 -type f
来源：http://dln.yuanzhike.top

[R45] 批量删除
来源：http://iyi.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://fny.zycfv.cn

[R46] 递归替换文件内容
来源：http://fbo.dianchejie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bqf.zhoulong.xyz

[R47] sed 单行替换
来源：http://szl.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://nmc.shzxlz.cn

[R48] awk 取指定列
来源：http://pig.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://nxi.316326.xyz

[R49] awk 带条件
来源：http://jlr.pengpengdd.cyou

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oso.cucudq.cn

[R50] awk 求和
来源：http://gxs.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://jsl.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://jwz.mhx1999.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ofh.tianlin.xyz

[R52] 统计行数
来源：http://mjj.daxiang520.top

wc -l a.txt
来源：http://crg.vehdjk.com

[R53] 查看文件头与实时尾
来源：http://kwg.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yny.gzhubu.top

[R54] 比较两个文件
来源：http://xuv.wangshuangyany.cn

diff a.txt b.txt
来源：http://xjc.nanxuanxn.top

[R55] 压缩与解压
来源：http://iho.yj202588.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yle.xuetiantiany.cn

[R56] 远程拷贝
来源：http://zor.zhijiandao.cn

scp file user@host:/path/
来源：http://qge.ehwqpu.com

[R57] 远程执行命令
来源：http://hcp.dianchejie.cn

ssh user@host 'uptime'
来源：http://viv.zhongyouzk.top

[R58] 下载文件
来源：http://pgt.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cpq.chenlongwang.top

[R59] 发 POST JSON
来源：http://grq.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uvn.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://bvt.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://inu.cqqwz.cn

[R61] 磁盘占用
来源：http://hlm.zdbjq.cn

df -h;  du -sh *
来源：http://qwu.xingfuxueyuan.xyz

[R62] 找最占空间的文件
来源：http://vcj.hongshengwenyu.top

du -ah . | sort -rh | head -10
来源：http://ewh.jqgufenzy.top

[R63] 内存与进程
来源：http://awx.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://lue.havefunace.top

[R64] 结束进程
来源：http://ouq.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://axd.yongpay.top

[R65] 查看端口占用
来源：http://qot.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pwe.mhx1999.top

[R66] 定时任务
来源：http://oah.yanxiufei.cn

crontab -e;  crontab -l
来源：http://vwc.daria6918.cn

[R67] 生成随机十六进制串
来源：http://xja.jinqigufen.top

openssl rand -hex 16
来源：http://rfg.zhixingplan.top

[R68] 计算文件校验值
来源：http://ehx.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://sso.cheryme.top

[R69] 生成随机密码
来源：http://dot.sweek.top

head -c 16 /dev/urandom | base64
来源：http://amv.ppjwa.cn

[R70] 时间戳与互转
来源：http://qvn.andypj.xyz

date +%s;  date -d @1700000000
来源：http://wdq.yonumen.top

[R71] 日期格式化
来源：http://mea.yongpay.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zge.shzxlz.cn

[R72] 等待端口就绪
来源：http://rve.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://suc.316326.xyz

[R73] 分割大日志
来源：http://wyc.yuxming.cn

split -l 1000 big.log part_
来源：http://osw.shangyingyoupin.top

[R74] 批量重命名
来源：http://hpx.zhoulong.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vxb.chenlongwang.top

[R75] 导出环境变量
来源：http://gym.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://pgl.bjfxy.top

[R76] 使用临时文件
来源：http://qup.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lxq.xingfuxueyuan.xyz

[R77] 读取用户输入
来源：http://iar.ehwqpu.com

read -rp "请输入: " ans
来源：http://ile.ydjk.org.cn

[R78] 交互式菜单
来源：http://phn.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vfp.ydjk.org.cn

[R79] 解析命令行选项
来源：http://ngi.nanxinkj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yqc.birdmap.top

[R80] 查看脚本执行耗时
来源：http://nco.yuanzhike.top

time ./run.sh
来源：http://uyn.xylfe.cn

================================================================================
来源：http://sxg.redwolf501.top

S. C / C++ 专题
来源：http://gng.xinyue.icu

================================================================================
来源：http://fsi.ehwqpu.com

[S01] C：Hello World
来源：http://xsn.meibo888.top

#include <stdio.h>
来源：http://aso.andypj.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://qgs.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://sub.yj20258.top

int a = 10; printf("%d\n", a);
来源：http://rzo.gaohongyu789.top

[S03] C：读入整数
来源：http://ubq.wangdashe.top

int x; scanf("%d", &x);
来源：http://nyn.pengpengdd.cyou

[S04] C：字符串复制
来源：http://cpz.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://qsa.kuanghao11.cn

[S05] C：字符串长度
来源：http://yih.ppjwa.cn

strlen(s)
来源：http://ski.pycfn.com

[S06] C：字符串比较
来源：http://uus.ehwqpu.com

strcmp(a, b) == 0
来源：http://uzu.9152youxi.cn

[S07] C：数组遍历求和
来源：http://aun.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ulb.xingfuxueyuan.xyz

[S08] C：动态内存分配与释放
来源：http://ixt.epnwcf.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qrr.guannengcc.top

[S09] C：结构体定义与初始化
来源：http://qzb.sweek.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zmi.fehbvm.com

[S10] C：指针与解引用
来源：http://zjh.nanxuanxn.top

int *p = &a;  *p = 5;
来源：http://rvz.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://phl.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://grl.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://imq.zdqjudy.top

fclose(f);
来源：http://pot.birdmap.top

[S12] C：写文件
来源：http://dzo.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bui.ydjk.org.cn

[S13] C：宏定义
来源：http://uah.sweek.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rwq.xuetiantiany.cn

[S14] C：枚举
来源：http://htx.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://rui.birdmap.top

[S15] C：类型转换
来源：http://rgf.smart0.xyz

(double) a / b
来源：http://rmc.cashguo.top

[S16] C：位操作置位
来源：http://hap.jianghu66.top

x |= (1 << 3);
来源：http://huw.iojbl.cn

[S17] C：安全拼接字符串
来源：http://mtl.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cnu.yangfankeji.com

[S18] C：命令行参数
来源：http://zmn.sufxvd.cn

int main(int argc, char **argv)
来源：http://wct.jinqigufen.top

[S19] C：快速排序
来源：http://shc.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://olv.xziqi.cn

[S20] C：二分查找
来源：http://ghf.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://thw.shuidangran.top

[S21] C：字符类别判断
来源：http://mke.uphjek.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jkv.jinghuilouyu.cn

[S22] C：字符串转数字
来源：http://zrk.fehbvm.com

atoi("42");  strtod("3.14", NULL);
来源：http://bog.yj20258.top

[S23] C：随机数
来源：http://erh.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hrn.kuanghao11.cn

[S24] C：获取本地时间
来源：http://emk.vqdsnc.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pmn.haohaochexian.top

[S25] C：内存拷贝
来源：http://euh.jqgfzy.top

memcpy(dst, src, n);
来源：http://ogz.snrcjt.cn

[S26] C：内存清零
来源：http://ohv.sxryk.cn

memset(a, 0, sizeof a);
来源：http://pel.pengpengdd.cyou

[S27] C：定义常量
来源：http://mih.hnqzz.top

const double PI = 3.14159;
来源：http://haz.chenlongwang.top

[S28] C：静态变量
来源：http://cjl.hammf.cn

static int counter = 0;
来源：http://myr.wangshuangyany.cn

[S29] C：变参函数
来源：http://env.havefunace.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nzk.aibaodan.cn

[S30] C：头文件保护
来源：http://clu.yuxming.cn

#ifndef X_H
来源：http://cyq.fengsongda.top

#define X_H
来源：http://gjn.daria6918.cn

#endif
来源：http://jfn.guannengcc.top

[S31] C++：Hello World
来源：http://lhw.gaohongyu789.top

#include <iostream>
来源：http://chf.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://khi.zhijiandao.cn

[S32] C++：字符串
来源：http://bdi.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://iwi.ctjpmb.com

[S33] C++：vector 增删
来源：http://sye.birdmap.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zxc.smart0.xyz

[S34] C++：遍历 vector
来源：http://qeu.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://xyy.xingfuxueyuan.xyz

[S35] C++：map
来源：http://vab.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bfa.cqqwz.cn

[S36] C++：unordered_map
来源：http://slf.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kgp.zhixingplan.top

[S37] C++：set
来源：http://spq.hesvh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://asb.52xcode.cn

[S38] C++：排序
来源：http://eib.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://yil.ivvv.top

[S39] C++：自定义比较器排序
来源：http://lge.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fao.nwbrower.top

[S40] C++：查找元素
来源：http://gyf.zhengqikj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lss.zycfv.cn

[S41] C++：类与构造函数
来源：http://zwk.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://scu.tian-w.cn

[S42] C++：继承与虚函数
来源：http://mpj.jinqigfzy.top

class B : public Base { public: void f() override {} };
来源：http://twe.gotoacloud.top

[S43] C++：智能指针
来源：http://sax.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://wef.xuetiantiany.cn

[S44] C++：引用传参
来源：http://han.shanyushiyangtech.top

void inc(int &x) { ++x; }
来源：http://jhj.zhoulong.xyz

[S45] C++：lambda
来源：http://afi.jyoumei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gcq.quarkkingdee.top

[S46] C++：函数模板
来源：http://xyc.hywenlv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zgk.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://hns.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yao.jiagoushi.top

[S48] C++：逐行读文件
来源：http://wvk.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uvv.yangfankeji.com

while (std::getline(in, line)) { }
来源：http://ddy.shanyushiyangtech.top

[S49] C++：写文件
来源：http://xzr.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sex.fktsv.cn

[S50] C++：格式化数字
来源：http://bnm.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nhr.gotoacloud.top

[S51] C++：显式类型转换
来源：http://nir.ehwqpu.com

static_cast<double>(a) / b
来源：http://ytz.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://jlk.fktsv.cn

int size() const noexcept { return n_; }
来源：http://ulx.yanxiufei.cn

[S53] C++：移动语义
来源：http://ltr.shangyingyoupin.top

std::vector<int> w = std::move(v);
来源：http://oxz.hywenlv.cn

[S54] C++：异常处理
来源：http://ngm.aibaodan.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gxn.bbcook.cn

[S55] C++：结构化绑定
来源：http://ufb.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wls.tanke756.top

[S56] C++：optional
来源：http://kgh.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hkd.ydjk.org.cn

[S57] C++：编译期常量
来源：http://ceo.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://ayg.fanxiaobao.xyz

[S58] C++：命名空间
来源：http://muu.cdnleiting.top

namespace ns { int f() { return 1; } }
来源：http://odv.fengsongda.top

[S59] C++：静态断言
来源：http://wtm.ehwqpu.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bjo.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://gwp.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rpn.andypj.xyz

================================================================================
来源：http://bmt.quarkkingdee.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bjr.hywenlv.cn

================================================================================
来源：http://hey.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://ybx.zhiwuduotai.top

println("Hello")
来源：http://hhm.wangdashe.top

[T02] Kotlin：变量
来源：http://tpm.havefunace.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hvd.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://tiy.yj20258.top

"值: $b"
来源：http://mzw.hammf.cn

[T04] Kotlin：空安全
来源：http://reh.feifeiyinyue.top

val n: String? = null;  n?.length
来源：http://wqy.xuetiantiany.cn


<!-- 参考信息 -->