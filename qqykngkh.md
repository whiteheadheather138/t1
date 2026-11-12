代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://bht.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gzm.pengpengdd.cyou

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eay.ivvv.top

[Q89] 判断表是否存在
来源：http://plg.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gil.xingfuxueyuan.xyz

[Q90] 生成序号列
来源：http://ycx.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://grr.hammf.cn

================================================================================
来源：http://eik.yongpay.top

R. Bash 专题
来源：http://utc.yonumen.top

================================================================================
来源：http://niy.dashuyun.cn

[R01] shebang 与严格模式
来源：http://qmr.shanyushiyangtech.top

#!/usr/bin/env bash
来源：http://zza.cheryme.top

set -euo pipefail
来源：http://jta.jinghuilouyu.cn

[R02] 变量赋值与使用
来源：http://ets.nanxinkj.top

name="Tom"; echo "$name"
来源：http://voh.quarkkingdee.top

[R03] 只读变量
来源：http://mvq.yueranfly.top

readonly PI=3.14
来源：http://mgz.hesvh.cn

[R04] 位置参数
来源：http://udj.fktsv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xsl.zdbjq.cn

[R05] 参数默认值
来源：http://kue.jqgfzy.top

name="${1:-default}"
来源：http://zsq.andypj.xyz

[R06] 判断命令是否存在
来源：http://eob.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vre.feifeiyinyue.top

[R07] if 判断文件
来源：http://xlq.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gal.sysykeji.top

[R08] 数值比较
来源：http://sms.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://wki.iojbl.cn

[R09] 字符串比较
来源：http://nai.9152youxi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://asc.zhiwuduotai.top

[R10] 正则匹配
来源：http://dqa.hongshengwenyu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wcy.tian-w.cn

[R11] case 多分支
来源：http://doe.fehbvm.com

case "$1" in
来源：http://bdp.epnwcf.com

start) echo "启动" ;;
来源：http://syq.haohaochexian.top

stop)  echo "停止" ;;
来源：http://ksl.wangdashe.top

*)     echo "未知命令" ;;
来源：http://iiv.jqgfzy.top

esac
来源：http://kqy.xuanzx.com

[R12] for 遍历文件
来源：http://dst.xylfe.cn

for f in *.txt; do echo "$f"; done
来源：http://qxu.ivvv.top

[R13] for 计数循环
来源：http://asg.vehdjk.com

for i in {1..10}; do echo "$i"; done
来源：http://nfa.gogol.net.cn

[R14] C 风格 for
来源：http://axp.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://phk.nwbrower.top

[R15] while 逐行读文件
来源：http://szx.yuxming.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rts.zhixingplan.top

[R16] until 等待条件
来源：http://kjc.fengsongda.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://myg.yuanzhike.top

[R17] 数组定义与取值
来源：http://zgl.aizwys.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cyu.cucudq.cn

[R18] 遍历数组
来源：http://rtw.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vxq.sweek.top

[R19] 数组长度
来源：http://wko.ivvv.top

echo "${#arr[@]}"
来源：http://aoh.zhengqikj.top

[R20] 关联数组（字典）
来源：http://dyu.hfpthk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://peu.smart0.xyz

[R21] 字符串长度
来源：http://cwi.jinqigfzy.top

echo "${#s}"
来源：http://ryx.andypj.xyz

[R22] 截取子串
来源：http://syw.daria6918.cn

echo "${s:0:5}"
来源：http://nzy.dianchejie.cn

[R23] 字符串替换
来源：http://hky.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jjj.cashguo.top

[R24] 大小写转换
来源：http://jzt.quarkkingdee.top

echo "${s^^}"; echo "${s,,}"
来源：http://pqd.9152youxi.cn

[R25] 去后缀 / 去前缀
来源：http://bqk.hammf.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hqm.jyoumei.cn

[R26] 命令替换
来源：http://jgz.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://kop.shanyushiyangtech.top

[R27] 算术展开
来源：http://eiu.yj202588.top

echo $((1 + 2 * 3))
来源：http://fya.guannengcc.top

[R28] 浮点运算
来源：http://lav.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://sec.sjlbkw.cn

[R29] 定义函数
来源：http://vzf.c1oappe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://muj.xinyue.icu

[R30] 函数返回状态码
来源：http://gbj.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://yiv.zdbjq.cn

[R31] 局部变量
来源：http://shn.gaohongyu789.top

f() { local x=1; echo "$x"; }
来源：http://gfh.ydzc1.top

[R32] 参数个数校验
来源：http://cpi.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cpl.shanyushiyangkeji.top

[R33] 捕获错误并提示行号
来源：http://rzs.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://acb.zhiwuduotai.top

[R34] 退出时清理
来源：http://hyr.birdmap.top

trap 'rm -f "$tmp"' EXIT
来源：http://yqz.zdqjudy.top

[R35] 后台执行并等待
来源：http://kxb.snrcjt.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vjx.bbcook.cn

[R36] 并发执行多个任务
来源：http://qpp.daxiang520.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bdy.hfpthk.cn

[R37] 把输出赋给变量
来源：http://hwp.yj20258888.top

files=$(ls -1)
来源：http://wkm.cheryme.top

[R38] 管道串联
来源：http://zsx.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://uva.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://fgo.ehwqpu.com

cmd > out.log 2>&1
来源：http://qmh.haohaochexian.top

[R40] 追加写日志
来源：http://ihz.havefunace.top

echo "log" >> out.log
来源：http://tqw.cucudq.cn

[R41] 丢弃输出
来源：http://kec.yj20258888.top

cmd >/dev/null 2>&1
来源：http://tyb.gzhubu.top

[R42] 输入重定向
来源：http://nkx.zdbjq.cn

wc -l < a.txt
来源：http://wwt.daria6918.cn

[R43] 按名字查找文件
来源：http://jbf.jqgufenzy.top

find . -name "*.log" -type f
来源：http://evx.fzhhl.top

[R44] 按修改时间查找
来源：http://qfp.bjfxy.top

find . -mtime -7 -type f
来源：http://fmf.dianchejie.cn

[R45] 批量删除
来源：http://jpl.tianlin.xyz

find . -name "*.tmp" -delete
来源：http://rkv.hysaishi.cn

[R46] 递归替换文件内容
来源：http://mqn.ydjk.org.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zuz.vqdsnc.cn

[R47] sed 单行替换
来源：http://hen.meibo888.top

sed -i 's/foo/bar/g' a.txt
来源：http://gnv.shzxlz.cn

[R48] awk 取指定列
来源：http://bah.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://uua.cashguo.top

[R49] awk 带条件
来源：http://wnj.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xhc.hesvh.cn

[R50] awk 求和
来源：http://rnj.uphjek.com

awk '{s += $2} END {print s}' a.txt
来源：http://unz.yj20258.top

[R51] 排序去重取前几
来源：http://jwn.zdqjudy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://azb.mhx1999.top

[R52] 统计行数
来源：http://bmg.jqgfzy.top

wc -l a.txt
来源：http://fvh.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://lqw.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://usc.fktsv.cn

[R54] 比较两个文件
来源：http://rlk.nwbrower.top

diff a.txt b.txt
来源：http://bae.kuanghao11.cn

[R55] 压缩与解压
来源：http://ryw.sxryk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qbt.jiagoushi.top

[R56] 远程拷贝
来源：http://cdr.iojbl.cn

scp file user@host:/path/
来源：http://zxc.dashuyun.cn

[R57] 远程执行命令
来源：http://nsa.aizwys.cn

ssh user@host 'uptime'
来源：http://fxv.ctjpmb.com

[R58] 下载文件
来源：http://hyb.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yyi.vqdsnc.cn

[R59] 发 POST JSON
来源：http://bbl.mhx1999.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qzm.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://bee.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ykm.gotoacloud.top

[R61] 磁盘占用
来源：http://gxe.quarkkingdee.top

df -h;  du -sh *
来源：http://art.yj20258888.top

[R62] 找最占空间的文件
来源：http://ndq.ppjwa.cn

du -ah . | sort -rh | head -10
来源：http://srj.hnxiangtu.top

[R63] 内存与进程
来源：http://lix.c1oappe.top

free -h;  ps aux | grep nginx
来源：http://tis.snrcjt.cn

[R64] 结束进程
来源：http://loc.fanxiaobao.xyz

kill -9 $(pgrep -f app.py)
来源：http://eeo.cucudq.cn

[R65] 查看端口占用
来源：http://adn.jinqigufen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xxl.sweek.top

[R66] 定时任务
来源：http://sjs.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://muf.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://nwh.nanxinkj.top

openssl rand -hex 16
来源：http://awv.pycfn.com

[R68] 计算文件校验值
来源：http://wpp.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lcs.dianchejie.cn

[R69] 生成随机密码
来源：http://vxr.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://nhh.fzhhl.top

[R70] 时间戳与互转
来源：http://iqg.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://yhu.zdbjq.cn

[R71] 日期格式化
来源：http://vld.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ceq.yangfankeji.com

[R72] 等待端口就绪
来源：http://gth.hongshengwenyu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wdo.xingfuxueyuan.xyz

[R73] 分割大日志
来源：http://dza.0kj1m.cn

split -l 1000 big.log part_
来源：http://qyw.yanxiufei.cn

[R74] 批量重命名
来源：http://icr.pycfn.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gur.hysaishi.cn

[R75] 导出环境变量
来源：http://tlv.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://weq.yueranfly.top

[R76] 使用临时文件
来源：http://tdt.jqgfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hjy.shanyushiyangtech.top

[R77] 读取用户输入
来源：http://xzt.hammf.cn

read -rp "请输入: " ans
来源：http://gzl.wangshuangyany.cn

[R78] 交互式菜单
来源：http://zwt.mhx1999.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fuv.ybcxt.top

[R79] 解析命令行选项
来源：http://xbe.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cvl.fktsv.cn

[R80] 查看脚本执行耗时
来源：http://fud.yonumen.top

time ./run.sh
来源：http://bfi.xuanzx.com

================================================================================
来源：http://yab.sjlbkw.cn

S. C / C++ 专题
来源：http://ffn.ivvv.top

================================================================================
来源：http://uok.tian-w.cn

[S01] C：Hello World
来源：http://vrh.andypj.xyz

#include <stdio.h>
来源：http://gef.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rvo.hesvh.cn

[S02] C：变量与格式化输出
来源：http://wlb.zhongyouzk.top

int a = 10; printf("%d\n", a);
来源：http://whf.yongpay.top

[S03] C：读入整数
来源：http://hfd.jinqigufen.top

int x; scanf("%d", &x);
来源：http://rip.gogol.net.cn

[S04] C：字符串复制
来源：http://pqi.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://vfz.mhx1999.top

[S05] C：字符串长度
来源：http://gws.hammf.cn

strlen(s)
来源：http://dgh.gaohongyu789.top

[S06] C：字符串比较
来源：http://fih.dianchejie.cn

strcmp(a, b) == 0
来源：http://qhx.yangfankeji.com

[S07] C：数组遍历求和
来源：http://uhu.sufxvd.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mla.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://nzp.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ifc.aibaodan.cn

[S09] C：结构体定义与初始化
来源：http://mfn.snrcjt.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tht.snrcjt.cn

[S10] C：指针与解引用
来源：http://udv.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://mrk.nanxinkj.top

[S11] C：逐行读文件
来源：http://far.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://mjc.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ygs.jianghu66.top

fclose(f);
来源：http://hew.fktsv.cn

[S12] C：写文件
来源：http://rbo.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mcf.hywenlv.cn

[S13] C：宏定义
来源：http://hcs.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://foj.sysykeji.top

[S14] C：枚举
来源：http://rtc.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://qlf.vqdsnc.cn

[S15] C：类型转换
来源：http://swo.xingfuxueyuan.xyz

(double) a / b
来源：http://khm.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://lor.zhoulong.xyz

x |= (1 << 3);
来源：http://dbb.zhaomingkeji.xyz

[S17] C：安全拼接字符串
来源：http://udq.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ibd.ywan-chungtsiang.top

[S18] C：命令行参数
来源：http://jaz.yanxiufei.cn

int main(int argc, char **argv)
来源：http://ojt.nanxinkj.top

[S19] C：快速排序
来源：http://luc.daria6918.cn

qsort(a, n, sizeof(int), cmp);
来源：http://koi.jianghu66.top

[S20] C：二分查找
来源：http://xsv.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gvw.zhongyouzk.top

[S21] C：字符类别判断
来源：http://wcr.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oem.zhixingplan.top

[S22] C：字符串转数字
来源：http://njm.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://trn.pycfn.com

[S23] C：随机数
来源：http://utv.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ymf.fehbvm.com

[S24] C：获取本地时间
来源：http://jas.ybcxt.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uvs.yuxming.cn

[S25] C：内存拷贝
来源：http://cgw.hesvh.cn

memcpy(dst, src, n);
来源：http://ywq.jinqigufen.top

[S26] C：内存清零
来源：http://oqj.nanxuanxn.top

memset(a, 0, sizeof a);
来源：http://hbe.quarkkingdee.top

[S27] C：定义常量
来源：http://fju.svipenyu.cn

const double PI = 3.14159;
来源：http://ehk.jlsjyb.cn

[S28] C：静态变量
来源：http://awa.tarul.cn

static int counter = 0;
来源：http://kfo.bbcook.cn

[S29] C：变参函数
来源：http://ewe.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uam.zhiwuduotai.top

[S30] C：头文件保护
来源：http://plu.fehbvm.com

#ifndef X_H
来源：http://arq.fehbvm.com

#define X_H
来源：http://tbr.sweek.top

#endif
来源：http://jhc.dianchejie.cn

[S31] C++：Hello World
来源：http://fpc.kuanghao11.cn

#include <iostream>
来源：http://myq.zdqjudy.top

int main() { std::cout << "Hello\n"; }
来源：http://ktk.hnxiangtu.top

[S32] C++：字符串
来源：http://qvx.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://efm.sxryk.cn

[S33] C++：vector 增删
来源：http://fte.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qbe.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://xle.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://urm.c1oappe.top

[S35] C++：map
来源：http://ern.ppjwa.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hpd.yanxiufei.cn

[S36] C++：unordered_map
来源：http://tzi.yvedp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kgt.jinghuilouyu.cn

[S37] C++：set
来源：http://dik.hnxiangtu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cug.dianchejie.cn

[S38] C++：排序
来源：http://juj.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://fxt.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://yfb.gotoacloud.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://izn.zycfv.cn

[S40] C++：查找元素
来源：http://brw.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zbc.redwolf501.top

[S41] C++：类与构造函数
来源：http://epl.quarkkingdee.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://szq.nwbrower.top

[S42] C++：继承与虚函数
来源：http://sma.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://iqj.fktsv.cn

[S43] C++：智能指针
来源：http://nih.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://ixz.jqgfzy.top

[S44] C++：引用传参
来源：http://sax.aizwys.cn

void inc(int &x) { ++x; }
来源：http://kgn.yvedp.cn

[S45] C++：lambda
来源：http://hwf.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://unu.cucudq.cn

[S46] C++：函数模板
来源：http://pwo.guowangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kxg.316326.xyz

[S47] C++：结构化绑定遍历
来源：http://gqc.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xsg.wangdashe.top

[S48] C++：逐行读文件
来源：http://iku.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tfb.ehwqpu.com

while (std::getline(in, line)) { }
来源：http://sgu.yj20258.top

[S49] C++：写文件
来源：http://yzx.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gos.ivvv.top

[S50] C++：格式化数字
来源：http://jao.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cnk.xuanzx.com

[S51] C++：显式类型转换
来源：http://gjv.xuanzx.com

static_cast<double>(a) / b
来源：http://lcp.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://emk.52xcode.cn

int size() const noexcept { return n_; }
来源：http://rhm.9152youxi.cn

[S53] C++：移动语义
来源：http://ana.yanxiufei.cn

std::vector<int> w = std::move(v);
来源：http://yns.quarkkingdee.top

[S54] C++：异常处理
来源：http://fvw.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sbo.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://uau.yvedp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mwk.dianchejie.cn

[S56] C++：optional
来源：http://upd.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sly.daria6918.cn

[S57] C++：编译期常量
来源：http://sqm.chenjidiqi.icu

constexpr int N = 10;
来源：http://bfq.jqgufenzy.top

[S58] C++：命名空间
来源：http://anm.nanxuanxn.top


<!-- 参考信息 -->