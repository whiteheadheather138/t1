代发 wailian999

R. Bash 专题
来源：http://npn.jyoumei.cn

================================================================================
来源：http://pgl.svipenyu.cn

[R01] shebang 与严格模式
来源：http://owq.316326.xyz

#!/usr/bin/env bash
来源：http://uur.c1oappe.top

set -euo pipefail
来源：http://zes.jiagoushi.top

[R02] 变量赋值与使用
来源：http://jyu.jqgfzy.top

name="Tom"; echo "$name"
来源：http://tri.52xcode.cn

[R03] 只读变量
来源：http://wbt.hnxiangtu.top

readonly PI=3.14
来源：http://fck.cashguo.top

[R04] 位置参数
来源：http://ebg.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cix.chenjidiqi.icu

[R05] 参数默认值
来源：http://hiw.nwbrower.top

name="${1:-default}"
来源：http://fmt.aibaodan.cn

[R06] 判断命令是否存在
来源：http://koi.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xvc.dashuyun.cn

[R07] if 判断文件
来源：http://auj.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tje.52xcode.cn

[R08] 数值比较
来源：http://vmc.cdnleiting.top

if (( a > b )); then echo "a 更大"; fi
来源：http://oaw.shuidangran.top

[R09] 字符串比较
来源：http://xfn.316326.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wyb.316326.xyz

[R10] 正则匹配
来源：http://lzx.meibo888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pgp.ivvv.top

[R11] case 多分支
来源：http://thb.chenzaomai.com

case "$1" in
来源：http://obx.redwolf501.top

start) echo "启动" ;;
来源：http://hwx.zhixingplan.top

stop)  echo "停止" ;;
来源：http://nve.dianchejie.cn

*)     echo "未知命令" ;;
来源：http://yto.iojbl.cn

esac
来源：http://khr.tianlin.xyz

[R12] for 遍历文件
来源：http://lxv.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://kmi.hysaishi.cn

[R13] for 计数循环
来源：http://olq.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://oip.zhixingplan.top

[R14] C 风格 for
来源：http://mci.svipenyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ngy.52xcode.cn

[R15] while 逐行读文件
来源：http://ogv.0kj1m.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mck.iojbl.cn

[R16] until 等待条件
来源：http://avx.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aum.fehbvm.com

[R17] 数组定义与取值
来源：http://asj.zhoulong.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://hqi.jiagoushi.top

[R18] 遍历数组
来源：http://mee.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://spm.gzhubu.top

[R19] 数组长度
来源：http://xql.zdbjq.cn

echo "${#arr[@]}"
来源：http://jaw.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://hmf.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://njv.hywenlv.cn

[R21] 字符串长度
来源：http://eig.shuidangran.top

echo "${#s}"
来源：http://xet.feifeiyinyue.top

[R22] 截取子串
来源：http://cbh.quarkkingdee.top

echo "${s:0:5}"
来源：http://kdf.hnqzz.top

[R23] 字符串替换
来源：http://zai.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kzb.xinyue.icu

[R24] 大小写转换
来源：http://tdf.9152youxi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xzc.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://bly.yj20258888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bri.uphjek.com

[R26] 命令替换
来源：http://kjr.aibaodan.cn

now=$(date +%F); echo "$now"
来源：http://vhg.fanxiaobao.xyz

[R27] 算术展开
来源：http://xpg.uphjek.com

echo $((1 + 2 * 3))
来源：http://jlx.zycfv.cn

[R28] 浮点运算
来源：http://tre.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://edv.shuidangran.top

[R29] 定义函数
来源：http://mgk.hfpthk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vso.guowangkeji.top

[R30] 函数返回状态码
来源：http://hkd.uphjek.com

f() { return 0; }; f || echo "失败了"
来源：http://wvo.yfazqb.com

[R31] 局部变量
来源：http://qgw.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://nny.yongpay.top

[R32] 参数个数校验
来源：http://tda.hnqzz.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mzi.52xcode.cn

[R33] 捕获错误并提示行号
来源：http://rrn.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aaf.vehdjk.com

[R34] 退出时清理
来源：http://gcu.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://emi.daria6918.cn

[R35] 后台执行并等待
来源：http://arw.epnwcf.com

sleep 5 & pid=$!; wait "$pid"
来源：http://mrx.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://xov.gogol.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://srb.cqqwz.cn

[R37] 把输出赋给变量
来源：http://ayd.zhengqikj.top

files=$(ls -1)
来源：http://drd.guannengcc.top

[R38] 管道串联
来源：http://rcq.jinyuanbaomall.cn

cat a.txt | grep -i error | wc -l
来源：http://fdm.vqdsnc.cn

[R39] 重定向标准输出与错误
来源：http://jlg.epnwcf.com

cmd > out.log 2>&1
来源：http://guc.nanxuanxn.top

[R40] 追加写日志
来源：http://hsb.hfpthk.cn

echo "log" >> out.log
来源：http://jqp.fktsv.cn

[R41] 丢弃输出
来源：http://wxb.yfazqb.com

cmd >/dev/null 2>&1
来源：http://glj.guannengcc.top

[R42] 输入重定向
来源：http://inl.zdqjudy.top

wc -l < a.txt
来源：http://yej.hnqzz.top

[R43] 按名字查找文件
来源：http://qxw.zdbjq.cn

find . -name "*.log" -type f
来源：http://vom.vehdjk.com

[R44] 按修改时间查找
来源：http://jmc.fehbvm.com

find . -mtime -7 -type f
来源：http://hoj.zhongyouzk.top

[R45] 批量删除
来源：http://itw.ydzc1.top

find . -name "*.tmp" -delete
来源：http://vdx.0kj1m.cn

[R46] 递归替换文件内容
来源：http://pvn.yanxiufei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://icq.jlsjyb.cn

[R47] sed 单行替换
来源：http://xdn.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://uce.yueranfly.top

[R48] awk 取指定列
来源：http://srm.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://omy.ydzc1.top

[R49] awk 带条件
来源：http://obs.chenjidiqi.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aup.iojbl.cn

[R50] awk 求和
来源：http://ypz.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://lbz.ydjk.org.cn

[R51] 排序去重取前几
来源：http://nya.hcnkem.com

sort a.txt | uniq -c | sort -rn | head
来源：http://gub.gotoacloud.top

[R52] 统计行数
来源：http://igf.xingfuxueyuan.xyz

wc -l a.txt
来源：http://cnw.316326.xyz

[R53] 查看文件头与实时尾
来源：http://bab.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://een.fktsv.cn

[R54] 比较两个文件
来源：http://wxl.fehbvm.com

diff a.txt b.txt
来源：http://irt.bbcook.cn

[R55] 压缩与解压
来源：http://sba.chenjidiqi.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zqj.tanke756.top

[R56] 远程拷贝
来源：http://noh.zhengqikj.top

scp file user@host:/path/
来源：http://aax.hysaishi.cn

[R57] 远程执行命令
来源：http://jju.mhx1999.top

ssh user@host 'uptime'
来源：http://naz.52xcode.cn

[R58] 下载文件
来源：http://ydc.ydzc1.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://izq.ehwqpu.com

[R59] 发 POST JSON
来源：http://xlx.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jvo.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://lql.uphjek.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blv.zhiwuduotai.top

[R61] 磁盘占用
来源：http://uvw.yuanzhike.top

df -h;  du -sh *
来源：http://ihq.sxryk.cn

[R62] 找最占空间的文件
来源：http://nzw.hnxiangtu.top

du -ah . | sort -rh | head -10
来源：http://ppz.cashguo.top

[R63] 内存与进程
来源：http://abs.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://ujk.bbcook.cn

[R64] 结束进程
来源：http://uvj.yj20258888.top

kill -9 $(pgrep -f app.py)
来源：http://ymn.sysykeji.top

[R65] 查看端口占用
来源：http://nem.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://thy.hesvh.cn

[R66] 定时任务
来源：http://hlc.tian-w.cn

crontab -e;  crontab -l
来源：http://esi.cdnleiting.top

[R67] 生成随机十六进制串
来源：http://qvo.ppjwa.cn

openssl rand -hex 16
来源：http://mcj.fzhhl.top

[R68] 计算文件校验值
来源：http://bnm.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lcy.cqqwz.cn

[R69] 生成随机密码
来源：http://dbz.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://xpk.fktsv.cn

[R70] 时间戳与互转
来源：http://rah.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://fmi.fehbvm.com

[R71] 日期格式化
来源：http://pcj.hnqzz.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ahh.kuanghao11.cn

[R72] 等待端口就绪
来源：http://wik.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zxr.fehbvm.com

[R73] 分割大日志
来源：http://fpn.havefunace.top

split -l 1000 big.log part_
来源：http://iiy.vehdjk.com

[R74] 批量重命名
来源：http://fhn.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tbu.quarkkingdee.top

[R75] 导出环境变量
来源：http://yjs.sysykeji.top

export PATH="$HOME/bin:$PATH"
来源：http://yef.yvedp.cn

[R76] 使用临时文件
来源：http://gcl.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dfd.zdqjudy.top

[R77] 读取用户输入
来源：http://nex.ppjwa.cn

read -rp "请输入: " ans
来源：http://ajh.jqgufenzy.top

[R78] 交互式菜单
来源：http://zrz.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cyb.cashguo.top

[R79] 解析命令行选项
来源：http://bxh.jianghu66.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://twq.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://aeh.yueranfly.top

time ./run.sh
来源：http://ydm.ydjk.org.cn

================================================================================
来源：http://cly.fehbvm.com

S. C / C++ 专题
来源：http://oyf.0kj1m.cn

================================================================================
来源：http://wkj.mhx1999.top

[S01] C：Hello World
来源：http://swi.kuanghao11.cn

#include <stdio.h>
来源：http://bde.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uba.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://huk.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://lzs.jinqigfzy.top

[S03] C：读入整数
来源：http://wib.ctjpmb.com

int x; scanf("%d", &x);
来源：http://kis.pycfn.com

[S04] C：字符串复制
来源：http://hmn.wangshuangyany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ity.zhongyouzk.top

[S05] C：字符串长度
来源：http://gji.cdnleiting.top

strlen(s)
来源：http://ngk.ydjk.org.cn

[S06] C：字符串比较
来源：http://arc.xziqi.cn

strcmp(a, b) == 0
来源：http://enf.zhengqikj.top

[S07] C：数组遍历求和
来源：http://ihi.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zwp.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://bjj.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://alr.cdnleiting.top

[S09] C：结构体定义与初始化
来源：http://vgo.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://equ.quarkkingdee.top

[S10] C：指针与解引用
来源：http://fnp.yj202588.top

int *p = &a;  *p = 5;
来源：http://xfe.yanxiufei.cn

[S11] C：逐行读文件
来源：http://nbl.tarul.cn

FILE *f = fopen("a.txt", "r");
来源：http://rto.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://oqw.zhiwuduotai.top

fclose(f);
来源：http://uaa.xinyue.icu

[S12] C：写文件
来源：http://ama.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jla.jianghu66.top

[S13] C：宏定义
来源：http://wnk.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://shl.shanyushiyangkeji.top

[S14] C：枚举
来源：http://irw.hnxiangtu.top

enum Color { RED, GREEN, BLUE };
来源：http://jkh.hnqzz.top

[S15] C：类型转换
来源：http://dow.yangfankeji.com

(double) a / b
来源：http://xvf.dashuyun.cn

[S16] C：位操作置位
来源：http://cxr.hesvh.cn

x |= (1 << 3);
来源：http://sbj.epnwcf.com

[S17] C：安全拼接字符串
来源：http://kdm.shuidangran.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eim.yfazqb.com

[S18] C：命令行参数
来源：http://xye.sxryk.cn

int main(int argc, char **argv)
来源：http://uwi.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://fec.aibaodan.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iml.kuanghao11.cn

[S20] C：二分查找
来源：http://xul.shangyingyoupin.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xjy.zdqjudy.top

[S21] C：字符类别判断
来源：http://jpn.52xcode.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xck.shangyingyoupin.top

[S22] C：字符串转数字
来源：http://nkg.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dku.dashuyun.cn

[S23] C：随机数
来源：http://ehk.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eio.hysaishi.cn

[S24] C：获取本地时间
来源：http://fzp.pengpengdd.cyou

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uhc.gotoacloud.top

[S25] C：内存拷贝
来源：http://xyf.yuxming.cn

memcpy(dst, src, n);
来源：http://huk.shangyingyoupin.top

[S26] C：内存清零
来源：http://shr.0kj1m.cn

memset(a, 0, sizeof a);
来源：http://dqo.cdnleiting.top

[S27] C：定义常量
来源：http://twr.xylfe.cn

const double PI = 3.14159;
来源：http://rja.cdnleiting.top

[S28] C：静态变量
来源：http://tgx.jinghuilouyu.cn

static int counter = 0;
来源：http://ofa.pengpengdd.cyou

[S29] C：变参函数
来源：http://tzd.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ped.zycfv.cn

[S30] C：头文件保护
来源：http://suw.aizwys.cn

#ifndef X_H
来源：http://ftf.shanyushiyangtech.top

#define X_H
来源：http://juo.jinyuanbaomall.cn

#endif
来源：http://fej.daria6918.cn

[S31] C++：Hello World
来源：http://pwz.shanyushiyangtech.top

#include <iostream>
来源：http://bij.zycfv.cn

int main() { std::cout << "Hello\n"; }
来源：http://dei.feifeiyinyue.top

[S32] C++：字符串
来源：http://wwl.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://tlo.ppjwa.cn

[S33] C++：vector 增删
来源：http://wab.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xuw.fzhhl.top

[S34] C++：遍历 vector
来源：http://sug.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://hry.hywenlv.cn

[S35] C++：map
来源：http://wku.dashuyun.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hri.zdqjudy.top

[S36] C++：unordered_map
来源：http://qjh.sjlbkw.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://itw.daria6918.cn

[S37] C++：set
来源：http://oft.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://axz.gogol.net.cn

[S38] C++：排序
来源：http://lun.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://wdw.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://njn.fehbvm.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jns.zhengqikj.top

[S40] C++：查找元素
来源：http://wlf.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://emd.epnwcf.com

[S41] C++：类与构造函数
来源：http://kut.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zvg.yj202588.top

[S42] C++：继承与虚函数
来源：http://bfl.sufxvd.cn

class B : public Base { public: void f() override {} };
来源：http://tyj.cheryme.top

[S43] C++：智能指针
来源：http://mxl.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://ptn.bbcook.cn

[S44] C++：引用传参
来源：http://vjb.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://ole.c1oappe.top

[S45] C++：lambda
来源：http://sdi.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://ggy.chenzaomai.com

[S46] C++：函数模板
来源：http://jad.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fnx.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://moh.meibo888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hwt.birdmap.top

[S48] C++：逐行读文件
来源：http://ssd.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vbs.52xcode.cn

while (std::getline(in, line)) { }
来源：http://zrk.shzxlz.cn

[S49] C++：写文件
来源：http://qwm.zdqjudy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pao.sweek.top

[S50] C++：格式化数字
来源：http://xso.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eqw.nanxinkj.top

[S51] C++：显式类型转换
来源：http://kzc.zdbjq.cn

static_cast<double>(a) / b
来源：http://iru.xylfe.cn

[S52] C++：const 与 noexcept
来源：http://wvl.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://nnp.jlsjyb.cn

[S53] C++：移动语义
来源：http://ean.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://hbe.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://ljf.yvedp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gsl.jqgfzy.top

[S55] C++：结构化绑定
来源：http://tkm.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://abk.zdqjudy.top

[S56] C++：optional
来源：http://nrv.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xmo.cheryme.top

[S57] C++：编译期常量
来源：http://abi.zhijiandao.cn

constexpr int N = 10;
来源：http://wip.dashuyun.cn

[S58] C++：命名空间
来源：http://qlu.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://zrz.chenjidiqi.icu

[S59] C++：静态断言
来源：http://pkp.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://flo.vehdjk.com

[S60] C++：遍历并删除元素
来源：http://dec.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://chv.ywan-chungtsiang.top

================================================================================
来源：http://feh.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tqm.hammf.cn

================================================================================
来源：http://ewu.9152youxi.cn


<!-- 参考信息 -->