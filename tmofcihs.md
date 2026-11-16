代发 wailian999

[Q82] 字符长度与字节长度
来源：http://bwt.shangyingyoupin.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xya.jlsjyb.cn

[Q83] 大小写转换
来源：http://usp.hnqzz.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tyq.zycfv.cn

[Q84] 去除首尾空格
来源：http://giz.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://pil.hnxiangtu.top

[Q85] 数值取整
来源：http://fcp.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ymp.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://zby.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ipu.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://btz.c1oappe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tgd.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://oye.aizwys.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://akh.tian-w.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jdg.aibaodan.cn

[Q89] 判断表是否存在
来源：http://vxx.hnxiangtu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yhi.tian-w.cn

[Q90] 生成序号列
来源：http://lcz.9152youxi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ncq.chenlongwang.top

================================================================================
来源：http://gew.hnxiangtu.top

R. Bash 专题
来源：http://cqe.jiagoushi.top

================================================================================
来源：http://pgo.gaohongyu789.top

[R01] shebang 与严格模式
来源：http://enk.wangdashe.top

#!/usr/bin/env bash
来源：http://dnz.zhiwuduotai.top

set -euo pipefail
来源：http://nkz.redwolf501.top

[R02] 变量赋值与使用
来源：http://icr.sweek.top

name="Tom"; echo "$name"
来源：http://qln.shuidangran.top

[R03] 只读变量
来源：http://cga.jqgfzy.top

readonly PI=3.14
来源：http://txn.fengsongda.top

[R04] 位置参数
来源：http://add.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sao.daria6918.cn

[R05] 参数默认值
来源：http://wsp.ctjpmb.com

name="${1:-default}"
来源：http://ctz.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://qrt.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kxi.kuanghao11.cn

[R07] if 判断文件
来源：http://hol.jyoumei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iro.gzhubu.top

[R08] 数值比较
来源：http://hkg.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://iyr.jinghuilouyu.cn

[R09] 字符串比较
来源：http://oji.jyoumei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vel.nanxinkj.top

[R10] 正则匹配
来源：http://zil.zhongyouzk.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xvl.nanxuanxn.top

[R11] case 多分支
来源：http://kdj.yvedp.cn

case "$1" in
来源：http://ifj.jinyuanbaomall.cn

start) echo "启动" ;;
来源：http://kim.xinyue.icu

stop)  echo "停止" ;;
来源：http://bwn.hnqzz.top

*)     echo "未知命令" ;;
来源：http://zue.jinyuanbaomall.cn

esac
来源：http://qck.gotoacloud.top

[R12] for 遍历文件
来源：http://ndr.feifeiyinyue.top

for f in *.txt; do echo "$f"; done
来源：http://hyh.hcnkem.com

[R13] for 计数循环
来源：http://mmr.hywenlv.cn

for i in {1..10}; do echo "$i"; done
来源：http://ndb.vqdsnc.cn

[R14] C 风格 for
来源：http://ofo.svipenyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dis.zhiwuduotai.top

[R15] while 逐行读文件
来源：http://lhk.gotoacloud.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nck.c1oappe.top

[R16] until 等待条件
来源：http://mvg.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ixu.chenlongwang.top

[R17] 数组定义与取值
来源：http://gqb.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://epa.zhaomingkeji.xyz

[R18] 遍历数组
来源：http://jzr.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bom.shanyushiyangkeji.top

[R19] 数组长度
来源：http://oyp.jqgufenzy.top

echo "${#arr[@]}"
来源：http://trz.yongpay.top

[R20] 关联数组（字典）
来源：http://qtp.cashguo.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hwz.yj202588.top

[R21] 字符串长度
来源：http://zon.yonumen.top

echo "${#s}"
来源：http://klx.dashuyun.cn

[R22] 截取子串
来源：http://cbe.yanxiufei.cn

echo "${s:0:5}"
来源：http://ssr.hnxiangtu.top

[R23] 字符串替换
来源：http://vju.andypj.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wow.ppjwa.cn

[R24] 大小写转换
来源：http://wjc.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://shu.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://hbr.shangyingyoupin.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jwp.9152youxi.cn

[R26] 命令替换
来源：http://hlf.jinghuilouyu.cn

now=$(date +%F); echo "$now"
来源：http://bxr.yuxming.cn

[R27] 算术展开
来源：http://vwt.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://iqs.zhiwuduotai.top

[R28] 浮点运算
来源：http://pjo.zdqjudy.top

echo "scale=2; 10/3" | bc
来源：http://efx.cqqwz.cn

[R29] 定义函数
来源：http://nre.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wot.jinqigfzy.top

[R30] 函数返回状态码
来源：http://hhp.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://stv.hcnkem.com

[R31] 局部变量
来源：http://wgu.zhiwuduotai.top

f() { local x=1; echo "$x"; }
来源：http://qeu.cucudq.cn

[R32] 参数个数校验
来源：http://vkh.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eve.shanyushiyangtech.top

[R33] 捕获错误并提示行号
来源：http://eyn.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dut.nanxinkj.top

[R34] 退出时清理
来源：http://syl.wangshuangyany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uqq.yfazqb.com

[R35] 后台执行并等待
来源：http://vni.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://vjl.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://ttu.c1oappe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mwf.cashguo.top

[R37] 把输出赋给变量
来源：http://kpi.wangdashe.top

files=$(ls -1)
来源：http://hye.ydzc1.top

[R38] 管道串联
来源：http://vvx.vqdsnc.cn

cat a.txt | grep -i error | wc -l
来源：http://scv.shangyingyoupin.top

[R39] 重定向标准输出与错误
来源：http://dlj.tianlin.xyz

cmd > out.log 2>&1
来源：http://pbt.jiagoushi.top

[R40] 追加写日志
来源：http://wbx.yongpay.top

echo "log" >> out.log
来源：http://aar.vqdsnc.cn

[R41] 丢弃输出
来源：http://kis.52xcode.cn

cmd >/dev/null 2>&1
来源：http://orz.pengpengdd.cyou

[R42] 输入重定向
来源：http://qvz.tanke756.top

wc -l < a.txt
来源：http://sei.316326.xyz

[R43] 按名字查找文件
来源：http://uie.tianlin.xyz

find . -name "*.log" -type f
来源：http://bpf.jyoumei.cn

[R44] 按修改时间查找
来源：http://ihs.yueranfly.top

find . -mtime -7 -type f
来源：http://yxh.haohaochexian.top

[R45] 批量删除
来源：http://bdc.yvedp.cn

find . -name "*.tmp" -delete
来源：http://wei.uphjek.com

[R46] 递归替换文件内容
来源：http://zuq.bjfxy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tvj.fzhhl.top

[R47] sed 单行替换
来源：http://zip.cheryme.top

sed -i 's/foo/bar/g' a.txt
来源：http://dna.hesvh.cn

[R48] awk 取指定列
来源：http://wyz.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://oro.quarkkingdee.top

[R49] awk 带条件
来源：http://uvs.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cuq.hammf.cn

[R50] awk 求和
来源：http://vkf.gaohongyu789.top

awk '{s += $2} END {print s}' a.txt
来源：http://knb.jqgufenzy.top

[R51] 排序去重取前几
来源：http://xkf.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pnx.fehbvm.com

[R52] 统计行数
来源：http://upc.316326.xyz

wc -l a.txt
来源：http://vyk.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://jsg.cucudq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://umf.bjfxy.top

[R54] 比较两个文件
来源：http://xnm.zhengqikj.top

diff a.txt b.txt
来源：http://owq.haohaochexian.top

[R55] 压缩与解压
来源：http://faj.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cmm.yj202588.top

[R56] 远程拷贝
来源：http://lga.nanxuanxn.top

scp file user@host:/path/
来源：http://rij.aibaodan.cn

[R57] 远程执行命令
来源：http://mvb.cucudq.cn

ssh user@host 'uptime'
来源：http://eji.dianchejie.cn

[R58] 下载文件
来源：http://joe.ctjpmb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fxx.316326.xyz

[R59] 发 POST JSON
来源：http://hzq.chenzaomai.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xyz.zhixingplan.top

[R60] 只看 HTTP 状态码
来源：http://iox.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mme.nanxuanxn.top

[R61] 磁盘占用
来源：http://nah.epnwcf.com

df -h;  du -sh *
来源：http://ujd.zhongyouzk.top

[R62] 找最占空间的文件
来源：http://ftj.jianghu66.top

du -ah . | sort -rh | head -10
来源：http://gvk.jinghuilouyu.cn

[R63] 内存与进程
来源：http://wwr.chenjidiqi.icu

free -h;  ps aux | grep nginx
来源：http://jzr.ydjk.org.cn

[R64] 结束进程
来源：http://ffg.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://sen.pycfn.com

[R65] 查看端口占用
来源：http://pkp.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sur.fengsongda.top

[R66] 定时任务
来源：http://qzl.hammf.cn

crontab -e;  crontab -l
来源：http://ppk.fengsongda.top

[R67] 生成随机十六进制串
来源：http://bbo.ydzc1.top

openssl rand -hex 16
来源：http://ezh.ydzc1.top

[R68] 计算文件校验值
来源：http://stz.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rhn.haohaochexian.top

[R69] 生成随机密码
来源：http://yuu.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://mli.xziqi.cn

[R70] 时间戳与互转
来源：http://nkp.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://jpe.hcnkem.com

[R71] 日期格式化
来源：http://mtk.nwbrower.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qoq.hfpthk.cn

[R72] 等待端口就绪
来源：http://yzt.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mon.pengpengdd.cyou

[R73] 分割大日志
来源：http://dhm.zhiwuduotai.top

split -l 1000 big.log part_
来源：http://zng.gzhubu.top

[R74] 批量重命名
来源：http://okk.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dqj.hongshengwenyu.top

[R75] 导出环境变量
来源：http://dcb.sxryk.cn

export PATH="$HOME/bin:$PATH"
来源：http://fth.ehwqpu.com

[R76] 使用临时文件
来源：http://mdj.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fdp.316326.xyz

[R77] 读取用户输入
来源：http://njv.uphjek.com

read -rp "请输入: " ans
来源：http://mei.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://agw.ehwqpu.com

select opt in a b c; do echo "$opt"; break; done
来源：http://fir.nwbrower.top

[R79] 解析命令行选项
来源：http://dqd.cucudq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lir.yonumen.top

[R80] 查看脚本执行耗时
来源：http://loh.smart0.xyz

time ./run.sh
来源：http://zjf.uphjek.com

================================================================================
来源：http://oss.sysykeji.top

S. C / C++ 专题
来源：http://bge.cdnleiting.top

================================================================================
来源：http://mkj.jinqigfzy.top

[S01] C：Hello World
来源：http://xes.pengpengdd.cyou

#include <stdio.h>
来源：http://ldv.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hrc.epnwcf.com

[S02] C：变量与格式化输出
来源：http://maa.jqgufenzy.top

int a = 10; printf("%d\n", a);
来源：http://vxt.yj20258.top

[S03] C：读入整数
来源：http://bsz.yangfankeji.com

int x; scanf("%d", &x);
来源：http://bya.havefunace.top

[S04] C：字符串复制
来源：http://zjt.wangshuangyany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vxy.tanke756.top

[S05] C：字符串长度
来源：http://cxy.shzxlz.cn

strlen(s)
来源：http://ilb.xingfuxueyuan.xyz

[S06] C：字符串比较
来源：http://rad.cdnleiting.top

strcmp(a, b) == 0
来源：http://hns.0kj1m.cn

[S07] C：数组遍历求和
来源：http://cdp.bjfxy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rao.quarkkingdee.top

[S08] C：动态内存分配与释放
来源：http://tid.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mpf.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://xlm.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sux.hfpthk.cn

[S10] C：指针与解引用
来源：http://mxs.pengpengdd.cyou

int *p = &a;  *p = 5;
来源：http://nta.iojbl.cn

[S11] C：逐行读文件
来源：http://mdq.yfazqb.com

FILE *f = fopen("a.txt", "r");
来源：http://eiu.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xxq.zhiwuduotai.top

fclose(f);
来源：http://zcd.havefunace.top

[S12] C：写文件
来源：http://bxm.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tzp.fzhhl.top

[S13] C：宏定义
来源：http://amv.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oym.andypj.xyz

[S14] C：枚举
来源：http://dep.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://olv.ydjk.org.cn

[S15] C：类型转换
来源：http://xzf.sweek.top

(double) a / b
来源：http://wgk.mhx1999.top

[S16] C：位操作置位
来源：http://kuv.zhengqikj.top

x |= (1 << 3);
来源：http://yxa.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://pzb.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hiu.fehbvm.com

[S18] C：命令行参数
来源：http://pyt.yj202588.top

int main(int argc, char **argv)
来源：http://xii.svipenyu.cn

[S19] C：快速排序
来源：http://nfq.vehdjk.com

qsort(a, n, sizeof(int), cmp);
来源：http://xde.jinqigfzy.top

[S20] C：二分查找
来源：http://gwk.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tov.c1oappe.top

[S21] C：字符类别判断
来源：http://pcf.shanyushiyangtech.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jwq.hywenlv.cn

[S22] C：字符串转数字
来源：http://fcp.xinyue.icu

atoi("42");  strtod("3.14", NULL);
来源：http://wvx.snrcjt.cn

[S23] C：随机数
来源：http://ihy.xuanzx.com

srand(time(NULL));  int r = rand() % 100;
来源：http://feq.gzhubu.top

[S24] C：获取本地时间
来源：http://fqx.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lub.ppjwa.cn

[S25] C：内存拷贝
来源：http://zsx.gogol.net.cn

memcpy(dst, src, n);
来源：http://rhq.sjlbkw.cn

[S26] C：内存清零
来源：http://pmg.birdmap.top

memset(a, 0, sizeof a);
来源：http://yja.jinqigfzy.top

[S27] C：定义常量
来源：http://nun.yueranfly.top

const double PI = 3.14159;
来源：http://dpn.meibo888.top

[S28] C：静态变量
来源：http://ezd.dashuyun.cn

static int counter = 0;
来源：http://dfg.shangyingyoupin.top

[S29] C：变参函数
来源：http://pgo.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cck.zhiwuduotai.top

[S30] C：头文件保护
来源：http://wqz.zhoulong.xyz

#ifndef X_H
来源：http://uig.guannengcc.top

#define X_H
来源：http://ube.wangdashe.top

#endif
来源：http://tsd.52xcode.cn

[S31] C++：Hello World
来源：http://xdn.mhx1999.top

#include <iostream>
来源：http://pfn.jqgfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://qaj.cashguo.top

[S32] C++：字符串
来源：http://ldb.tanke756.top

std::string s = "hi";  s += "!";
来源：http://owa.sufxvd.cn

[S33] C++：vector 增删
来源：http://gsb.tanke756.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rlu.sufxvd.cn

[S34] C++：遍历 vector
来源：http://brm.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://zgp.redwolf501.top

[S35] C++：map
来源：http://dgk.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iom.yj20258.top

[S36] C++：unordered_map
来源：http://uix.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bva.smart0.xyz

[S37] C++：set
来源：http://mca.pengpengdd.cyou

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pwm.daria6918.cn

[S38] C++：排序
来源：http://ely.sysykeji.top

std::sort(v.begin(), v.end());
来源：http://kxv.chenzaomai.com

[S39] C++：自定义比较器排序
来源：http://ebm.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iyp.hnxiangtu.top

[S40] C++：查找元素
来源：http://sqr.ybcxt.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ioy.0kj1m.cn

[S41] C++：类与构造函数
来源：http://eis.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pgi.ydjk.org.cn

[S42] C++：继承与虚函数
来源：http://icv.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://rll.nanxinkj.top

[S43] C++：智能指针
来源：http://vys.cqqwz.cn

auto p = std::make_unique<int>(5);
来源：http://znh.aizwys.cn

[S44] C++：引用传参
来源：http://mwt.dashuyun.cn

void inc(int &x) { ++x; }
来源：http://sco.havefunace.top

[S45] C++：lambda
来源：http://vmt.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kzw.shuidangran.top

[S46] C++：函数模板
来源：http://sgw.gotoacloud.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qwr.ivvv.top

[S47] C++：结构化绑定遍历
来源：http://cic.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://med.hnqzz.top

[S48] C++：逐行读文件
来源：http://ntp.shangyingyoupin.top

std::ifstream in("a.txt");  std::string line;
来源：http://guc.meibo888.top

while (std::getline(in, line)) { }
来源：http://ujt.hnqzz.top

[S49] C++：写文件
来源：http://txi.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://btr.hcnkem.com

[S50] C++：格式化数字
来源：http://rqi.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nej.shangyingyoupin.top

[S51] C++：显式类型转换
来源：http://dcy.zdbjq.cn

static_cast<double>(a) / b
来源：http://nfx.yongpay.top

[S52] C++：const 与 noexcept
来源：http://tev.iojbl.cn


<!-- 参考信息 -->