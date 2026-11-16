代发 wailian999

[Q82] 字符长度与字节长度
来源：http://tuy.bjfxy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hgi.zhongyouzk.top

[Q83] 大小写转换
来源：http://vkg.yj20258888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jrp.hywenlv.cn

[Q84] 去除首尾空格
来源：http://hfv.yongpay.top

SELECT TRIM(name) FROM users;
来源：http://oos.tanke756.top

[Q85] 数值取整
来源：http://eow.xziqi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://npd.hysaishi.cn

[Q86] 读取 JSON 字段
来源：http://nvg.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ocu.zycfv.cn

[Q87] JSON 字段做条件
来源：http://wod.andypj.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xrm.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://ezb.ivvv.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vut.ybcxt.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wzx.xuanzx.com

[Q89] 判断表是否存在
来源：http://xlf.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wdd.tanke756.top

[Q90] 生成序号列
来源：http://thv.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aag.yongpay.top

================================================================================
来源：http://ixd.hywenlv.cn

R. Bash 专题
来源：http://ksh.zhaomingkeji.xyz

================================================================================
来源：http://pyx.aibaodan.cn

[R01] shebang 与严格模式
来源：http://eqw.jinghuilouyu.cn

#!/usr/bin/env bash
来源：http://nkn.jyoumei.cn

set -euo pipefail
来源：http://uio.yanxiufei.cn

[R02] 变量赋值与使用
来源：http://xob.ppjwa.cn

name="Tom"; echo "$name"
来源：http://hci.tian-w.cn

[R03] 只读变量
来源：http://xzu.vehdjk.com

readonly PI=3.14
来源：http://bxx.svipenyu.cn

[R04] 位置参数
来源：http://qpt.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://amb.vehdjk.com

[R05] 参数默认值
来源：http://mvk.ehwqpu.com

name="${1:-default}"
来源：http://hxx.hnxiangtu.top

[R06] 判断命令是否存在
来源：http://cuc.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hez.chenjidiqi.icu

[R07] if 判断文件
来源：http://onk.haohaochexian.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ujv.tarul.cn

[R08] 数值比较
来源：http://xiy.fktsv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ami.vqdsnc.cn

[R09] 字符串比较
来源：http://ika.ppjwa.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ile.yangfankeji.com

[R10] 正则匹配
来源：http://gtu.jyoumei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ccu.hysaishi.cn

[R11] case 多分支
来源：http://xgg.shanyushiyangtech.top

case "$1" in
来源：http://sgh.fzhhl.top

start) echo "启动" ;;
来源：http://yaw.xinyue.icu

stop)  echo "停止" ;;
来源：http://zma.yangfankeji.com

*)     echo "未知命令" ;;
来源：http://shp.dianchejie.cn

esac
来源：http://fcs.52xcode.cn

[R12] for 遍历文件
来源：http://dtd.shzxlz.cn

for f in *.txt; do echo "$f"; done
来源：http://oce.snrcjt.cn

[R13] for 计数循环
来源：http://ktl.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://tnq.zhijiandao.cn

[R14] C 风格 for
来源：http://zda.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nvh.xziqi.cn

[R15] while 逐行读文件
来源：http://mmu.yuxming.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lsg.vehdjk.com

[R16] until 等待条件
来源：http://bvk.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sop.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://gvm.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://cgp.jiagoushi.top

[R18] 遍历数组
来源：http://qfe.dashuyun.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zek.yonumen.top

[R19] 数组长度
来源：http://gft.ehwqpu.com

echo "${#arr[@]}"
来源：http://xcw.dianchejie.cn

[R20] 关联数组（字典）
来源：http://fhn.zycfv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pya.xinyue.icu

[R21] 字符串长度
来源：http://mlf.gzhubu.top

echo "${#s}"
来源：http://jqe.hysaishi.cn

[R22] 截取子串
来源：http://ejp.havefunace.top

echo "${s:0:5}"
来源：http://ksi.yj20258.top

[R23] 字符串替换
来源：http://oxl.cqqwz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ass.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://bbi.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://iyj.sysykeji.top

[R25] 去后缀 / 去前缀
来源：http://ixk.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://uvs.zhoulong.xyz

[R26] 命令替换
来源：http://dvu.sweek.top

now=$(date +%F); echo "$now"
来源：http://rov.meibo888.top

[R27] 算术展开
来源：http://kyh.hcnkem.com

echo $((1 + 2 * 3))
来源：http://cfa.hongshengwenyu.top

[R28] 浮点运算
来源：http://jke.mhx1999.top

echo "scale=2; 10/3" | bc
来源：http://dto.jinghuilouyu.cn

[R29] 定义函数
来源：http://tor.bbcook.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xgz.jianghu66.top

[R30] 函数返回状态码
来源：http://chq.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://fll.feifeiyinyue.top

[R31] 局部变量
来源：http://wmj.ywan-chungtsiang.top

f() { local x=1; echo "$x"; }
来源：http://dud.dashuyun.cn

[R32] 参数个数校验
来源：http://qyl.iojbl.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nou.fzhhl.top

[R33] 捕获错误并提示行号
来源：http://ulu.jinyuanbaomall.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bsv.mhx1999.top

[R34] 退出时清理
来源：http://xaz.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qsi.snrcjt.cn

[R35] 后台执行并等待
来源：http://eej.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cro.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://lxh.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tir.fehbvm.com

[R37] 把输出赋给变量
来源：http://fhg.ydzc1.top

files=$(ls -1)
来源：http://hil.redwolf501.top

[R38] 管道串联
来源：http://ipw.quarkkingdee.top

cat a.txt | grep -i error | wc -l
来源：http://ite.xuanzx.com

[R39] 重定向标准输出与错误
来源：http://rsh.hywenlv.cn

cmd > out.log 2>&1
来源：http://kmk.zhoulong.xyz

[R40] 追加写日志
来源：http://bzp.hnqzz.top

echo "log" >> out.log
来源：http://psi.hnxiangtu.top

[R41] 丢弃输出
来源：http://rfs.yonumen.top

cmd >/dev/null 2>&1
来源：http://nrw.c1oappe.top

[R42] 输入重定向
来源：http://yjd.sysykeji.top

wc -l < a.txt
来源：http://piw.dianchejie.cn

[R43] 按名字查找文件
来源：http://wbo.zdqjudy.top

find . -name "*.log" -type f
来源：http://fbd.hywenlv.cn

[R44] 按修改时间查找
来源：http://hcd.vqdsnc.cn

find . -mtime -7 -type f
来源：http://irk.haohaochexian.top

[R45] 批量删除
来源：http://zoa.sweek.top

find . -name "*.tmp" -delete
来源：http://jnf.xylfe.cn

[R46] 递归替换文件内容
来源：http://awu.iojbl.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bne.aibaodan.cn

[R47] sed 单行替换
来源：http://cmt.meibo888.top

sed -i 's/foo/bar/g' a.txt
来源：http://ijz.xziqi.cn

[R48] awk 取指定列
来源：http://yxz.kuanghao11.cn

awk '{print $1, $3}' a.txt
来源：http://ehs.chenzaomai.com

[R49] awk 带条件
来源：http://ofm.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vkq.sysykeji.top

[R50] awk 求和
来源：http://ulk.jqgufenzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://ugu.yj20258888.top

[R51] 排序去重取前几
来源：http://fpt.ppjwa.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lwz.redwolf501.top

[R52] 统计行数
来源：http://agg.shanyushiyangtech.top

wc -l a.txt
来源：http://gxr.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://yqg.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mnh.yueranfly.top

[R54] 比较两个文件
来源：http://okh.sysykeji.top

diff a.txt b.txt
来源：http://goq.zhijiandao.cn

[R55] 压缩与解压
来源：http://jgg.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ovx.yfazqb.com

[R56] 远程拷贝
来源：http://aeu.birdmap.top

scp file user@host:/path/
来源：http://bdy.jinqigufen.top

[R57] 远程执行命令
来源：http://brb.hfpthk.cn

ssh user@host 'uptime'
来源：http://haw.shuidangran.top

[R58] 下载文件
来源：http://dit.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ydm.fehbvm.com

[R59] 发 POST JSON
来源：http://sfe.ywan-chungtsiang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://avn.dianchejie.cn

[R60] 只看 HTTP 状态码
来源：http://rwi.cdnleiting.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dqv.yueranfly.top

[R61] 磁盘占用
来源：http://szz.gotoacloud.top

df -h;  du -sh *
来源：http://yxj.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://nbb.yuanzhike.top

du -ah . | sort -rh | head -10
来源：http://bga.zdbjq.cn

[R63] 内存与进程
来源：http://cjr.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://okw.hysaishi.cn

[R64] 结束进程
来源：http://mpx.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://ykt.havefunace.top

[R65] 查看端口占用
来源：http://sbp.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cnv.snrcjt.cn

[R66] 定时任务
来源：http://deq.hnxiangtu.top

crontab -e;  crontab -l
来源：http://gzt.fanxiaobao.xyz

[R67] 生成随机十六进制串
来源：http://qav.havefunace.top

openssl rand -hex 16
来源：http://wbm.chenzaomai.com

[R68] 计算文件校验值
来源：http://zao.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://hfg.daxiang520.top

[R69] 生成随机密码
来源：http://keh.yvedp.cn

head -c 16 /dev/urandom | base64
来源：http://lkv.cqqwz.cn

[R70] 时间戳与互转
来源：http://ghr.fanxiaobao.xyz

date +%s;  date -d @1700000000
来源：http://hzm.shangyingyoupin.top

[R71] 日期格式化
来源：http://tvp.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yiw.zhixingplan.top

[R72] 等待端口就绪
来源：http://hxp.snrcjt.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://edr.smart0.xyz

[R73] 分割大日志
来源：http://xgq.fzhhl.top

split -l 1000 big.log part_
来源：http://fsx.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://mqx.xylfe.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dil.zhoulong.xyz

[R75] 导出环境变量
来源：http://kby.yuxming.cn

export PATH="$HOME/bin:$PATH"
来源：http://usv.cqqwz.cn

[R76] 使用临时文件
来源：http://fzm.pycfn.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rlo.zhixingplan.top

[R77] 读取用户输入
来源：http://bcm.shanyushiyangkeji.top

read -rp "请输入: " ans
来源：http://plr.jiagoushi.top

[R78] 交互式菜单
来源：http://dkk.aibaodan.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dfg.yvedp.cn

[R79] 解析命令行选项
来源：http://hwt.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tna.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://wnb.zhiwuduotai.top

time ./run.sh
来源：http://hvo.yj202588.top

================================================================================
来源：http://jhz.ehwqpu.com

S. C / C++ 专题
来源：http://fyj.guowangkeji.top

================================================================================
来源：http://rie.ehwqpu.com

[S01] C：Hello World
来源：http://jpa.ehwqpu.com

#include <stdio.h>
来源：http://yas.cucudq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xtg.yj20258888.top

[S02] C：变量与格式化输出
来源：http://lkz.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://trk.gzhubu.top

[S03] C：读入整数
来源：http://pih.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://nsc.hesvh.cn

[S04] C：字符串复制
来源：http://gui.ywan-chungtsiang.top

char dst[32]; strcpy(dst, "hi");
来源：http://yry.chenlongwang.top

[S05] C：字符串长度
来源：http://aog.zdbjq.cn

strlen(s)
来源：http://vwc.jinghuilouyu.cn

[S06] C：字符串比较
来源：http://oyh.xingfuxueyuan.xyz

strcmp(a, b) == 0
来源：http://ktp.jinyuanbaomall.cn

[S07] C：数组遍历求和
来源：http://alh.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ugm.quarkkingdee.top

[S08] C：动态内存分配与释放
来源：http://yng.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bjh.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://cmk.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nkp.zdqjudy.top

[S10] C：指针与解引用
来源：http://hwc.fktsv.cn

int *p = &a;  *p = 5;
来源：http://sjq.fehbvm.com

[S11] C：逐行读文件
来源：http://csh.sweek.top

FILE *f = fopen("a.txt", "r");
来源：http://ldg.hammf.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xsi.quarkkingdee.top

fclose(f);
来源：http://rcy.fktsv.cn

[S12] C：写文件
来源：http://itu.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zqg.hfpthk.cn

[S13] C：宏定义
来源：http://gha.xingfuxueyuan.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mic.guannengcc.top

[S14] C：枚举
来源：http://mvz.guannengcc.top

enum Color { RED, GREEN, BLUE };
来源：http://cnf.zhixingplan.top

[S15] C：类型转换
来源：http://jee.redwolf501.top

(double) a / b
来源：http://gnp.52xcode.cn

[S16] C：位操作置位
来源：http://ncg.yongpay.top

x |= (1 << 3);
来源：http://hwj.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://qkz.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hki.guannengcc.top

[S18] C：命令行参数
来源：http://dlb.hysaishi.cn

int main(int argc, char **argv)
来源：http://cmr.cqqwz.cn

[S19] C：快速排序
来源：http://eme.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://tge.chenjidiqi.icu

[S20] C：二分查找
来源：http://fep.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mpd.fengsongda.top

[S21] C：字符类别判断
来源：http://kgk.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bsw.9152youxi.cn

[S22] C：字符串转数字
来源：http://npl.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://qeh.9152youxi.cn

[S23] C：随机数
来源：http://zjx.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://izx.gzhubu.top

[S24] C：获取本地时间
来源：http://omr.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bvu.jiagoushi.top

[S25] C：内存拷贝
来源：http://stz.yanxiufei.cn

memcpy(dst, src, n);
来源：http://gmn.ybcxt.top

[S26] C：内存清零
来源：http://atg.aizwys.cn

memset(a, 0, sizeof a);
来源：http://ywg.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://eet.bjfxy.top

const double PI = 3.14159;
来源：http://nge.yj20258.top

[S28] C：静态变量
来源：http://zdu.fktsv.cn

static int counter = 0;
来源：http://djx.jqgfzy.top

[S29] C：变参函数
来源：http://hml.chenlongwang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gva.hysaishi.cn

[S30] C：头文件保护
来源：http://rcr.chenzaomai.com

#ifndef X_H
来源：http://vam.jlsjyb.cn

#define X_H
来源：http://mgi.sxryk.cn

#endif
来源：http://vmh.cashguo.top

[S31] C++：Hello World
来源：http://hzf.pengpengdd.cyou

#include <iostream>
来源：http://rkt.jinqigufen.top

int main() { std::cout << "Hello\n"; }
来源：http://idn.zhongyouzk.top

[S32] C++：字符串
来源：http://igs.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://bhr.hfpthk.cn

[S33] C++：vector 增删
来源：http://ssv.sjlbkw.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ywq.shanyushiyangkeji.top

[S34] C++：遍历 vector
来源：http://uve.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://yef.shangyingyoupin.top

[S35] C++：map
来源：http://aya.sysykeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vss.zhongyouzk.top

[S36] C++：unordered_map
来源：http://ejx.bjfxy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tuk.haohaochexian.top

[S37] C++：set
来源：http://zhl.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cyk.zycfv.cn

[S38] C++：排序
来源：http://etv.tian-w.cn

std::sort(v.begin(), v.end());
来源：http://tba.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://awz.svipenyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eun.havefunace.top

[S40] C++：查找元素
来源：http://bka.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lrq.havefunace.top

[S41] C++：类与构造函数
来源：http://byq.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ucl.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://mfu.wangshuangyany.cn

class B : public Base { public: void f() override {} };
来源：http://nlg.hnxiangtu.top

[S43] C++：智能指针
来源：http://rai.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://fpe.zdbjq.cn

[S44] C++：引用传参
来源：http://bxq.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://aqw.sjlbkw.cn

[S45] C++：lambda
来源：http://wog.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://civ.haohaochexian.top

[S46] C++：函数模板
来源：http://etk.yangfankeji.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uqh.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://nls.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bvq.ivvv.top

[S48] C++：逐行读文件
来源：http://xpl.yuxming.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qik.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://uht.shzxlz.cn

[S49] C++：写文件
来源：http://hjk.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tbf.ydjk.org.cn

[S50] C++：格式化数字
来源：http://sdf.epnwcf.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://phv.haohaochexian.top

[S51] C++：显式类型转换
来源：http://bxi.tian-w.cn

static_cast<double>(a) / b
来源：http://aia.shanyushiyangtech.top

[S52] C++：const 与 noexcept
来源：http://qjz.wangshuangyany.cn


<!-- 参考信息 -->