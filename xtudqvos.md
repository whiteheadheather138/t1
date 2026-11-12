代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://sxf.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sga.daria6918.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wob.yfazqb.com

[Q89] 判断表是否存在
来源：http://wch.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rtd.zdbjq.cn

[Q90] 生成序号列
来源：http://vin.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lok.fanxiaobao.xyz

================================================================================
来源：http://fog.c1oappe.top

R. Bash 专题
来源：http://iwd.sufxvd.cn

================================================================================
来源：http://rgi.shanyushiyangkeji.top

[R01] shebang 与严格模式
来源：http://ucz.wangdashe.top

#!/usr/bin/env bash
来源：http://nso.nanxinkj.top

set -euo pipefail
来源：http://xno.xziqi.cn

[R02] 变量赋值与使用
来源：http://fce.xingfuxueyuan.xyz

name="Tom"; echo "$name"
来源：http://vdr.yvedp.cn

[R03] 只读变量
来源：http://ups.hongshengwenyu.top

readonly PI=3.14
来源：http://ref.xuetiantiany.cn

[R04] 位置参数
来源：http://gzz.fktsv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sap.zhengqikj.top

[R05] 参数默认值
来源：http://pcp.xziqi.cn

name="${1:-default}"
来源：http://tiz.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://tzb.vqdsnc.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xwo.shangyingyoupin.top

[R07] if 判断文件
来源：http://blf.epnwcf.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pfv.dianchejie.cn

[R08] 数值比较
来源：http://xqf.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ejd.wangshuangyany.cn

[R09] 字符串比较
来源：http://knj.zdbjq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qyo.shzxlz.cn

[R10] 正则匹配
来源：http://hui.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://onq.zdbjq.cn

[R11] case 多分支
来源：http://xke.316326.xyz

case "$1" in
来源：http://uwf.zhengqikj.top

start) echo "启动" ;;
来源：http://xyg.daria6918.cn

stop)  echo "停止" ;;
来源：http://iul.hesvh.cn

*)     echo "未知命令" ;;
来源：http://ctf.jinqigfzy.top

esac
来源：http://ryi.zhiwuduotai.top

[R12] for 遍历文件
来源：http://mtg.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://ioi.hywenlv.cn

[R13] for 计数循环
来源：http://kxp.gaohongyu789.top

for i in {1..10}; do echo "$i"; done
来源：http://ork.ehwqpu.com

[R14] C 风格 for
来源：http://bik.zycfv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rlh.shanyushiyangkeji.top

[R15] while 逐行读文件
来源：http://hkp.jqgfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ncv.sysykeji.top

[R16] until 等待条件
来源：http://okz.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gry.ivvv.top

[R17] 数组定义与取值
来源：http://fiu.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://lgd.0kj1m.cn

[R18] 遍历数组
来源：http://qeh.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nwa.hongshengwenyu.top

[R19] 数组长度
来源：http://gmg.svipenyu.cn

echo "${#arr[@]}"
来源：http://txg.hnxiangtu.top

[R20] 关联数组（字典）
来源：http://zuo.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tdj.ydjk.org.cn

[R21] 字符串长度
来源：http://ulp.daxiang520.top

echo "${#s}"
来源：http://yyk.aibaodan.cn

[R22] 截取子串
来源：http://zyx.snrcjt.cn

echo "${s:0:5}"
来源：http://zcm.fengsongda.top

[R23] 字符串替换
来源：http://fyc.hcnkem.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://itz.jyoumei.cn

[R24] 大小写转换
来源：http://veu.0kj1m.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nds.epnwcf.com

[R25] 去后缀 / 去前缀
来源：http://wie.sysykeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jxb.guannengcc.top

[R26] 命令替换
来源：http://fuy.sxryk.cn

now=$(date +%F); echo "$now"
来源：http://gan.hnxiangtu.top

[R27] 算术展开
来源：http://pnw.shanyushiyangtech.top

echo $((1 + 2 * 3))
来源：http://wqn.chenlongwang.top

[R28] 浮点运算
来源：http://plt.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://xix.uphjek.com

[R29] 定义函数
来源：http://zjy.zhongyouzk.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kju.xinyue.icu

[R30] 函数返回状态码
来源：http://qwk.gaohongyu789.top

f() { return 0; }; f || echo "失败了"
来源：http://cdm.yueranfly.top

[R31] 局部变量
来源：http://whh.gotoacloud.top

f() { local x=1; echo "$x"; }
来源：http://kaz.sxryk.cn

[R32] 参数个数校验
来源：http://fhr.zhiwuduotai.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xvr.nwbrower.top

[R33] 捕获错误并提示行号
来源：http://goq.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tnw.cucudq.cn

[R34] 退出时清理
来源：http://fiq.jlsjyb.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ylp.zhijiandao.cn

[R35] 后台执行并等待
来源：http://ruu.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://agf.fktsv.cn

[R36] 并发执行多个任务
来源：http://eab.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jwk.snrcjt.cn

[R37] 把输出赋给变量
来源：http://xhq.smart0.xyz

files=$(ls -1)
来源：http://uty.jlsjyb.cn

[R38] 管道串联
来源：http://dal.cucudq.cn

cat a.txt | grep -i error | wc -l
来源：http://nns.jinyuanbaomall.cn

[R39] 重定向标准输出与错误
来源：http://qpk.zhijiandao.cn

cmd > out.log 2>&1
来源：http://yll.gzhubu.top

[R40] 追加写日志
来源：http://tqk.52xcode.cn

echo "log" >> out.log
来源：http://nbx.xuanzx.com

[R41] 丢弃输出
来源：http://sxy.xingfuxueyuan.xyz

cmd >/dev/null 2>&1
来源：http://wyw.guannengcc.top

[R42] 输入重定向
来源：http://plt.tanke756.top

wc -l < a.txt
来源：http://cgw.daria6918.cn

[R43] 按名字查找文件
来源：http://gae.hcnkem.com

find . -name "*.log" -type f
来源：http://iqj.0kj1m.cn

[R44] 按修改时间查找
来源：http://dqu.vqdsnc.cn

find . -mtime -7 -type f
来源：http://kyu.zhaomingkeji.xyz

[R45] 批量删除
来源：http://agi.sysykeji.top

find . -name "*.tmp" -delete
来源：http://eip.jqgufenzy.top

[R46] 递归替换文件内容
来源：http://xhl.tarul.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ygs.hnxiangtu.top

[R47] sed 单行替换
来源：http://ass.zhongyouzk.top

sed -i 's/foo/bar/g' a.txt
来源：http://gec.epnwcf.com

[R48] awk 取指定列
来源：http://ilz.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://mrg.iojbl.cn

[R49] awk 带条件
来源：http://eji.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tgj.tianlin.xyz

[R50] awk 求和
来源：http://zbg.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://swo.nanxuanxn.top

[R51] 排序去重取前几
来源：http://guq.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://dhj.ctjpmb.com

[R52] 统计行数
来源：http://bgc.hysaishi.cn

wc -l a.txt
来源：http://tyb.dianchejie.cn

[R53] 查看文件头与实时尾
来源：http://tbv.ctjpmb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rby.ydzc1.top

[R54] 比较两个文件
来源：http://pgu.haohaochexian.top

diff a.txt b.txt
来源：http://ojc.andypj.xyz

[R55] 压缩与解压
来源：http://czo.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://udc.kuanghao11.cn

[R56] 远程拷贝
来源：http://faz.smart0.xyz

scp file user@host:/path/
来源：http://gld.sweek.top

[R57] 远程执行命令
来源：http://goz.hnqzz.top

ssh user@host 'uptime'
来源：http://nzo.yj202588.top

[R58] 下载文件
来源：http://new.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hll.fanxiaobao.xyz

[R59] 发 POST JSON
来源：http://yep.zhaomingkeji.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xvs.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://glj.snrcjt.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qji.zdbjq.cn

[R61] 磁盘占用
来源：http://cqz.jlsjyb.cn

df -h;  du -sh *
来源：http://sdx.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://rdm.daria6918.cn

du -ah . | sort -rh | head -10
来源：http://yme.pycfn.com

[R63] 内存与进程
来源：http://vhi.xuanzx.com

free -h;  ps aux | grep nginx
来源：http://dtl.chenzaomai.com

[R64] 结束进程
来源：http://pcm.jyoumei.cn

kill -9 $(pgrep -f app.py)
来源：http://tvc.xingfuxueyuan.xyz

[R65] 查看端口占用
来源：http://bim.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rrw.wangdashe.top

[R66] 定时任务
来源：http://led.xylfe.cn

crontab -e;  crontab -l
来源：http://qad.xuanzx.com

[R67] 生成随机十六进制串
来源：http://deb.52xcode.cn

openssl rand -hex 16
来源：http://dlk.52xcode.cn

[R68] 计算文件校验值
来源：http://uyi.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rcp.uphjek.com

[R69] 生成随机密码
来源：http://udu.epnwcf.com

head -c 16 /dev/urandom | base64
来源：http://dzz.hcnkem.com

[R70] 时间戳与互转
来源：http://zkl.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://chj.wangdashe.top

[R71] 日期格式化
来源：http://whv.gzhubu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jqt.shzxlz.cn

[R72] 等待端口就绪
来源：http://hkd.redwolf501.top

until nc -z localhost 3306; do sleep 1; done
来源：http://axj.guowangkeji.top

[R73] 分割大日志
来源：http://awu.zdqjudy.top

split -l 1000 big.log part_
来源：http://faq.ivvv.top

[R74] 批量重命名
来源：http://hma.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dll.jiagoushi.top

[R75] 导出环境变量
来源：http://ryi.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://nzj.feifeiyinyue.top

[R76] 使用临时文件
来源：http://zjd.yuxming.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fed.dianchejie.cn

[R77] 读取用户输入
来源：http://xxk.yuanzhike.top

read -rp "请输入: " ans
来源：http://mms.ctjpmb.com

[R78] 交互式菜单
来源：http://ama.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mri.hysaishi.cn

[R79] 解析命令行选项
来源：http://tor.316326.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bnd.yvedp.cn

[R80] 查看脚本执行耗时
来源：http://ndi.tianlin.xyz

time ./run.sh
来源：http://xju.nanxinkj.top

================================================================================
来源：http://vxe.uphjek.com

S. C / C++ 专题
来源：http://otd.uphjek.com

================================================================================
来源：http://hkw.hfpthk.cn

[S01] C：Hello World
来源：http://cvb.guowangkeji.top

#include <stdio.h>
来源：http://nkp.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://jpp.hysaishi.cn

[S02] C：变量与格式化输出
来源：http://kiu.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://jzm.jyoumei.cn

[S03] C：读入整数
来源：http://oej.cdnleiting.top

int x; scanf("%d", &x);
来源：http://wtx.mhx1999.top

[S04] C：字符串复制
来源：http://oey.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pec.aizwys.cn

[S05] C：字符串长度
来源：http://lmh.uphjek.com

strlen(s)
来源：http://snz.hnxiangtu.top

[S06] C：字符串比较
来源：http://gnq.vehdjk.com

strcmp(a, b) == 0
来源：http://omw.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://yjv.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gtb.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://htu.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://klf.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://evs.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fcf.aizwys.cn

[S10] C：指针与解引用
来源：http://rex.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://emb.birdmap.top

[S11] C：逐行读文件
来源：http://zej.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://nct.hcnkem.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://raa.yvedp.cn

fclose(f);
来源：http://rqp.yuxming.cn

[S12] C：写文件
来源：http://ebr.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dxf.chenzaomai.com

[S13] C：宏定义
来源：http://hmy.gaohongyu789.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oet.ywan-chungtsiang.top

[S14] C：枚举
来源：http://krs.fehbvm.com

enum Color { RED, GREEN, BLUE };
来源：http://qhp.ydzc1.top

[S15] C：类型转换
来源：http://kmj.yfazqb.com

(double) a / b
来源：http://cwu.jqgfzy.top

[S16] C：位操作置位
来源：http://hqs.fanxiaobao.xyz

x |= (1 << 3);
来源：http://bil.ivvv.top

[S17] C：安全拼接字符串
来源：http://pot.ehwqpu.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wij.hnqzz.top

[S18] C：命令行参数
来源：http://iof.yonumen.top

int main(int argc, char **argv)
来源：http://fly.daria6918.cn

[S19] C：快速排序
来源：http://adk.shanyushiyangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://dvq.jlsjyb.cn

[S20] C：二分查找
来源：http://myz.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pmr.jianghu66.top

[S21] C：字符类别判断
来源：http://dep.hesvh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hth.zhijiandao.cn

[S22] C：字符串转数字
来源：http://ywq.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://wnn.chenzaomai.com

[S23] C：随机数
来源：http://eky.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dje.jqgufenzy.top

[S24] C：获取本地时间
来源：http://xda.smart0.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cjk.hnxiangtu.top

[S25] C：内存拷贝
来源：http://wcy.tanke756.top

memcpy(dst, src, n);
来源：http://hqp.tian-w.cn

[S26] C：内存清零
来源：http://kib.wangdashe.top

memset(a, 0, sizeof a);
来源：http://coq.havefunace.top

[S27] C：定义常量
来源：http://dbw.ybcxt.top

const double PI = 3.14159;
来源：http://rze.yj20258.top

[S28] C：静态变量
来源：http://aun.guowangkeji.top

static int counter = 0;
来源：http://azs.gogol.net.cn

[S29] C：变参函数
来源：http://gsp.chenzaomai.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ijl.aizwys.cn

[S30] C：头文件保护
来源：http://lzs.sweek.top

#ifndef X_H
来源：http://dvy.pycfn.com

#define X_H
来源：http://dck.zhijiandao.cn

#endif
来源：http://pqr.xuetiantiany.cn

[S31] C++：Hello World
来源：http://dcq.feifeiyinyue.top

#include <iostream>
来源：http://dem.hfpthk.cn

int main() { std::cout << "Hello\n"; }
来源：http://qac.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://mid.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://pxw.jianghu66.top

[S33] C++：vector 增删
来源：http://ipe.hnqzz.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bsz.sweek.top

[S34] C++：遍历 vector
来源：http://svh.yj20258888.top

for (auto &x : v) { std::cout << x; }
来源：http://uwj.fehbvm.com

[S35] C++：map
来源：http://mdj.aibaodan.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kqb.meibo888.top

[S36] C++：unordered_map
来源：http://ghb.havefunace.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vsk.feifeiyinyue.top

[S37] C++：set
来源：http://ohm.jqgfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ggg.yuanzhike.top

[S38] C++：排序
来源：http://lxg.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://tgq.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://nkj.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mkr.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://fgm.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qnr.aizwys.cn

[S41] C++：类与构造函数
来源：http://est.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://igt.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://dlg.yuanzhike.top

class B : public Base { public: void f() override {} };
来源：http://ovr.zhongyouzk.top

[S43] C++：智能指针
来源：http://wwy.daria6918.cn

auto p = std::make_unique<int>(5);
来源：http://ztz.yj202588.top

[S44] C++：引用传参
来源：http://scg.xziqi.cn

void inc(int &x) { ++x; }
来源：http://khi.jyoumei.cn

[S45] C++：lambda
来源：http://tkl.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://zer.birdmap.top

[S46] C++：函数模板
来源：http://tmi.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vaz.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://nth.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dmh.yonumen.top

[S48] C++：逐行读文件
来源：http://xyx.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://sfg.yueranfly.top

while (std::getline(in, line)) { }
来源：http://nkb.uphjek.com

[S49] C++：写文件
来源：http://gus.snrcjt.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fcz.hnxiangtu.top

[S50] C++：格式化数字
来源：http://zce.feifeiyinyue.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wsb.quarkkingdee.top

[S51] C++：显式类型转换
来源：http://bxg.jqgfzy.top

static_cast<double>(a) / b
来源：http://zqu.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://wuv.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://faa.tarul.cn

[S53] C++：移动语义
来源：http://btv.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://kts.cheryme.top

[S54] C++：异常处理
来源：http://tob.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ryw.cheryme.top

[S55] C++：结构化绑定
来源：http://rvp.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zvn.daxiang520.top

[S56] C++：optional
来源：http://ubz.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wrr.aibaodan.cn

[S57] C++：编译期常量
来源：http://hrc.nanxuanxn.top

constexpr int N = 10;
来源：http://das.fehbvm.com

[S58] C++：命名空间
来源：http://upj.fktsv.cn


<!-- 参考信息 -->