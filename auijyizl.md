代发 wailian999

[Q80] 字符串截取
来源：http://cgt.nanxuanxn.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xru.zhijiandao.cn

[Q81] 字符串替换
来源：http://idt.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://glz.sxryk.cn

[Q82] 字符长度与字节长度
来源：http://xii.sxryk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lvn.haohaochexian.top

[Q83] 大小写转换
来源：http://whr.cqqwz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rte.hcnkem.com

[Q84] 去除首尾空格
来源：http://dli.guowangkeji.top

SELECT TRIM(name) FROM users;
来源：http://gau.hnqzz.top

[Q85] 数值取整
来源：http://vfj.jinghuilouyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yto.shuidangran.top

[Q86] 读取 JSON 字段
来源：http://dju.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eii.yangfankeji.com

[Q87] JSON 字段做条件
来源：http://foq.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bjn.meibo888.top

[Q88] 行转列（条件聚合）
来源：http://mbz.hammf.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uhm.sufxvd.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bqk.iojbl.cn

[Q89] 判断表是否存在
来源：http://gwm.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tle.jlsjyb.cn

[Q90] 生成序号列
来源：http://zhn.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://glt.zdbjq.cn

================================================================================
来源：http://eaj.hongshengwenyu.top

R. Bash 专题
来源：http://lkw.hfpthk.cn

================================================================================
来源：http://bnm.ydzc1.top

[R01] shebang 与严格模式
来源：http://crh.vqdsnc.cn

#!/usr/bin/env bash
来源：http://xwb.ydzc1.top

set -euo pipefail
来源：http://tqv.hfpthk.cn

[R02] 变量赋值与使用
来源：http://obj.cdnleiting.top

name="Tom"; echo "$name"
来源：http://yjy.ehwqpu.com

[R03] 只读变量
来源：http://edl.fehbvm.com

readonly PI=3.14
来源：http://qiv.sufxvd.cn

[R04] 位置参数
来源：http://owy.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wyg.316326.xyz

[R05] 参数默认值
来源：http://juq.sufxvd.cn

name="${1:-default}"
来源：http://xas.hywenlv.cn

[R06] 判断命令是否存在
来源：http://szx.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uws.ywan-chungtsiang.top

[R07] if 判断文件
来源：http://ihk.vehdjk.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ckd.tarul.cn

[R08] 数值比较
来源：http://lyu.zhoulong.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://voa.52xcode.cn

[R09] 字符串比较
来源：http://xxo.jinghuilouyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hsf.hnxiangtu.top

[R10] 正则匹配
来源：http://zdv.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hsz.ehwqpu.com

[R11] case 多分支
来源：http://hba.ybcxt.top

case "$1" in
来源：http://emr.xuetiantiany.cn

start) echo "启动" ;;
来源：http://mij.iojbl.cn

stop)  echo "停止" ;;
来源：http://ygu.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://fgw.birdmap.top

esac
来源：http://vgk.chenjidiqi.icu

[R12] for 遍历文件
来源：http://vpw.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://roa.yangfankeji.com

[R13] for 计数循环
来源：http://jkj.yj20258888.top

for i in {1..10}; do echo "$i"; done
来源：http://koy.shuidangran.top

[R14] C 风格 for
来源：http://ypj.fehbvm.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dpp.gogol.net.cn

[R15] while 逐行读文件
来源：http://xys.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vwz.jiagoushi.top

[R16] until 等待条件
来源：http://aqq.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yng.ivvv.top

[R17] 数组定义与取值
来源：http://hod.jiagoushi.top

arr=(a b c); echo "${arr[0]}"
来源：http://lom.shanyushiyangkeji.top

[R18] 遍历数组
来源：http://tbu.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wmj.hammf.cn

[R19] 数组长度
来源：http://dyu.zycfv.cn

echo "${#arr[@]}"
来源：http://dqt.fengsongda.top

[R20] 关联数组（字典）
来源：http://fbl.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kue.pengpengdd.cyou

[R21] 字符串长度
来源：http://jmb.yongpay.top

echo "${#s}"
来源：http://yqn.nanxinkj.top

[R22] 截取子串
来源：http://fgm.hongshengwenyu.top

echo "${s:0:5}"
来源：http://pxh.uphjek.com

[R23] 字符串替换
来源：http://mla.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dld.fehbvm.com

[R24] 大小写转换
来源：http://vfb.hesvh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nkb.pycfn.com

[R25] 去后缀 / 去前缀
来源：http://pcu.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://drl.sjlbkw.cn

[R26] 命令替换
来源：http://aao.jlsjyb.cn

now=$(date +%F); echo "$now"
来源：http://sht.cucudq.cn

[R27] 算术展开
来源：http://zws.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://wia.jlsjyb.cn

[R28] 浮点运算
来源：http://zik.xziqi.cn

echo "scale=2; 10/3" | bc
来源：http://sxw.ctjpmb.com

[R29] 定义函数
来源：http://cbk.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yas.yonumen.top

[R30] 函数返回状态码
来源：http://nev.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://kse.jlsjyb.cn

[R31] 局部变量
来源：http://qip.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://gvt.haohaochexian.top

[R32] 参数个数校验
来源：http://urm.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vaj.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://nud.epnwcf.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jjx.sysykeji.top

[R34] 退出时清理
来源：http://dbd.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://jzz.fengsongda.top

[R35] 后台执行并等待
来源：http://tar.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dgy.hfpthk.cn

[R36] 并发执行多个任务
来源：http://ndo.nanxinkj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ptr.gzhubu.top

[R37] 把输出赋给变量
来源：http://ulh.jlsjyb.cn

files=$(ls -1)
来源：http://acw.shanyushiyangkeji.top

[R38] 管道串联
来源：http://egk.dianchejie.cn

cat a.txt | grep -i error | wc -l
来源：http://chk.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://sya.havefunace.top

cmd > out.log 2>&1
来源：http://qyx.yuanzhike.top

[R40] 追加写日志
来源：http://lrd.sysykeji.top

echo "log" >> out.log
来源：http://yqz.xziqi.cn

[R41] 丢弃输出
来源：http://fyy.shuidangran.top

cmd >/dev/null 2>&1
来源：http://pke.jinghuilouyu.cn

[R42] 输入重定向
来源：http://zop.hongshengwenyu.top

wc -l < a.txt
来源：http://yjx.52xcode.cn

[R43] 按名字查找文件
来源：http://jky.yuxming.cn

find . -name "*.log" -type f
来源：http://zxd.sufxvd.cn

[R44] 按修改时间查找
来源：http://mlp.vqdsnc.cn

find . -mtime -7 -type f
来源：http://scd.yj20258888.top

[R45] 批量删除
来源：http://nei.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://jxp.ywan-chungtsiang.top

[R46] 递归替换文件内容
来源：http://yrk.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wde.jqgfzy.top

[R47] sed 单行替换
来源：http://szr.hesvh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qpp.yj20258.top

[R48] awk 取指定列
来源：http://ufe.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://qyy.ybcxt.top

[R49] awk 带条件
来源：http://xro.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fvi.cdnleiting.top

[R50] awk 求和
来源：http://bst.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://agq.ppjwa.cn

[R51] 排序去重取前几
来源：http://yvi.zdbjq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ijr.jinqigufen.top

[R52] 统计行数
来源：http://myh.fehbvm.com

wc -l a.txt
来源：http://lyf.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://qvn.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://foy.quarkkingdee.top

[R54] 比较两个文件
来源：http://tgo.zhixingplan.top

diff a.txt b.txt
来源：http://ojk.chenjidiqi.icu

[R55] 压缩与解压
来源：http://mez.mhx1999.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bai.yonumen.top

[R56] 远程拷贝
来源：http://jwv.jlsjyb.cn

scp file user@host:/path/
来源：http://cal.ehwqpu.com

[R57] 远程执行命令
来源：http://sjw.wangdashe.top

ssh user@host 'uptime'
来源：http://lkk.epnwcf.com

[R58] 下载文件
来源：http://nyz.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jqi.zycfv.cn

[R59] 发 POST JSON
来源：http://pws.sxryk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pge.guowangkeji.top

[R60] 只看 HTTP 状态码
来源：http://aci.chenjidiqi.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bgt.xingfuxueyuan.xyz

[R61] 磁盘占用
来源：http://kqc.yvedp.cn

df -h;  du -sh *
来源：http://jwe.gogol.net.cn

[R62] 找最占空间的文件
来源：http://bnz.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://qnr.xylfe.cn

[R63] 内存与进程
来源：http://vjl.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://gsw.zhijiandao.cn

[R64] 结束进程
来源：http://pvx.quarkkingdee.top

kill -9 $(pgrep -f app.py)
来源：http://rex.shangyingyoupin.top

[R65] 查看端口占用
来源：http://okh.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://csb.shangyingyoupin.top

[R66] 定时任务
来源：http://iwb.uphjek.com

crontab -e;  crontab -l
来源：http://adx.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://vfe.hcnkem.com

openssl rand -hex 16
来源：http://cob.hcnkem.com

[R68] 计算文件校验值
来源：http://nwb.chenlongwang.top

sha256sum a.txt;  md5sum a.txt
来源：http://qnm.nanxuanxn.top

[R69] 生成随机密码
来源：http://krd.daxiang520.top

head -c 16 /dev/urandom | base64
来源：http://moe.yj202588.top

[R70] 时间戳与互转
来源：http://jyf.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://eaw.bbcook.cn

[R71] 日期格式化
来源：http://trz.nwbrower.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://opj.guannengcc.top

[R72] 等待端口就绪
来源：http://ghi.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://osw.jlsjyb.cn

[R73] 分割大日志
来源：http://efx.dianchejie.cn

split -l 1000 big.log part_
来源：http://ura.redwolf501.top

[R74] 批量重命名
来源：http://dmx.birdmap.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vcd.meibo888.top

[R75] 导出环境变量
来源：http://kro.vehdjk.com

export PATH="$HOME/bin:$PATH"
来源：http://ski.zhijiandao.cn

[R76] 使用临时文件
来源：http://iwc.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gcn.52xcode.cn

[R77] 读取用户输入
来源：http://wyh.yj20258888.top

read -rp "请输入: " ans
来源：http://lbl.mhx1999.top

[R78] 交互式菜单
来源：http://zbu.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ihh.yj202588.top

[R79] 解析命令行选项
来源：http://din.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://owi.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://rmy.hcnkem.com

time ./run.sh
来源：http://amf.nanxinkj.top

================================================================================
来源：http://hrk.jqgufenzy.top

S. C / C++ 专题
来源：http://gid.zhengqikj.top

================================================================================
来源：http://drc.yfazqb.com

[S01] C：Hello World
来源：http://cyt.cucudq.cn

#include <stdio.h>
来源：http://ofx.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rcs.ivvv.top

[S02] C：变量与格式化输出
来源：http://gln.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://gvv.guannengcc.top

[S03] C：读入整数
来源：http://ndq.yj20258888.top

int x; scanf("%d", &x);
来源：http://nas.cdnleiting.top

[S04] C：字符串复制
来源：http://lcw.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://frv.zdqjudy.top

[S05] C：字符串长度
来源：http://hgk.fktsv.cn

strlen(s)
来源：http://usk.yangfankeji.com

[S06] C：字符串比较
来源：http://vxs.cucudq.cn

strcmp(a, b) == 0
来源：http://sbh.shangyingyoupin.top

[S07] C：数组遍历求和
来源：http://ulu.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fem.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://zvk.nwbrower.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zno.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://kez.bjfxy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://glh.havefunace.top

[S10] C：指针与解引用
来源：http://blu.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://ind.yongpay.top

[S11] C：逐行读文件
来源：http://qqw.jinghuilouyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://wuj.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vgv.52xcode.cn

fclose(f);
来源：http://rzy.0kj1m.cn

[S12] C：写文件
来源：http://rmy.tianlin.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yoa.yueranfly.top

[S13] C：宏定义
来源：http://inb.bjfxy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jxu.ctjpmb.com

[S14] C：枚举
来源：http://lsk.nanxinkj.top

enum Color { RED, GREEN, BLUE };
来源：http://gco.hammf.cn

[S15] C：类型转换
来源：http://alq.cashguo.top

(double) a / b
来源：http://lud.ydzc1.top

[S16] C：位操作置位
来源：http://blo.yj20258888.top

x |= (1 << 3);
来源：http://cke.zhengqikj.top

[S17] C：安全拼接字符串
来源：http://jml.shuidangran.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gmz.feifeiyinyue.top

[S18] C：命令行参数
来源：http://hyb.yvedp.cn

int main(int argc, char **argv)
来源：http://ety.ydjk.org.cn

[S19] C：快速排序
来源：http://svj.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iiv.jqgufenzy.top

[S20] C：二分查找
来源：http://kho.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dzv.yuanzhike.top

[S21] C：字符类别判断
来源：http://cyn.zhongyouzk.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://smf.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://lcu.ywan-chungtsiang.top

atoi("42");  strtod("3.14", NULL);
来源：http://oax.dashuyun.cn

[S23] C：随机数
来源：http://mwv.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bem.yongpay.top

[S24] C：获取本地时间
来源：http://nqa.ydjk.org.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oqn.ctjpmb.com

[S25] C：内存拷贝
来源：http://gdb.vehdjk.com

memcpy(dst, src, n);
来源：http://ezp.ydjk.org.cn

[S26] C：内存清零
来源：http://ljk.yuxming.cn

memset(a, 0, sizeof a);
来源：http://ikh.ydzc1.top

[S27] C：定义常量
来源：http://hcg.zhijiandao.cn

const double PI = 3.14159;
来源：http://slc.316326.xyz

[S28] C：静态变量
来源：http://cor.yfazqb.com

static int counter = 0;
来源：http://nqq.ydzc1.top

[S29] C：变参函数
来源：http://woh.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://apt.birdmap.top

[S30] C：头文件保护
来源：http://sca.yj20258888.top

#ifndef X_H
来源：http://yeh.zhixingplan.top

#define X_H
来源：http://usm.hysaishi.cn

#endif
来源：http://fjo.meibo888.top

[S31] C++：Hello World
来源：http://jdi.hcnkem.com

#include <iostream>
来源：http://qyl.ydjk.org.cn

int main() { std::cout << "Hello\n"; }
来源：http://pkh.tianlin.xyz

[S32] C++：字符串
来源：http://xuu.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://qdc.redwolf501.top

[S33] C++：vector 增删
来源：http://xcy.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rxl.snrcjt.cn

[S34] C++：遍历 vector
来源：http://qnm.nwbrower.top

for (auto &x : v) { std::cout << x; }
来源：http://hgb.yj20258.top

[S35] C++：map
来源：http://wlr.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kmn.svipenyu.cn

[S36] C++：unordered_map
来源：http://awd.hammf.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ffa.andypj.xyz

[S37] C++：set
来源：http://vpv.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yin.smart0.xyz

[S38] C++：排序
来源：http://lsy.aizwys.cn

std::sort(v.begin(), v.end());
来源：http://off.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://oun.snrcjt.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ubo.vehdjk.com

[S40] C++：查找元素
来源：http://vdp.nanxuanxn.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wmy.cucudq.cn

[S41] C++：类与构造函数
来源：http://qyz.fanxiaobao.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wwb.epnwcf.com

[S42] C++：继承与虚函数
来源：http://vdp.jiagoushi.top

class B : public Base { public: void f() override {} };
来源：http://aue.sxryk.cn

[S43] C++：智能指针
来源：http://yhc.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://vzz.wangdashe.top

[S44] C++：引用传参
来源：http://gwf.jiagoushi.top

void inc(int &x) { ++x; }
来源：http://blb.hcnkem.com

[S45] C++：lambda
来源：http://cjj.vqdsnc.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oer.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://hsu.hcnkem.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vds.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://txg.gzhubu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ixf.tian-w.cn

[S48] C++：逐行读文件
来源：http://bfh.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://rvn.daxiang520.top

while (std::getline(in, line)) { }
来源：http://toa.jqgufenzy.top

[S49] C++：写文件
来源：http://uxy.jlsjyb.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://umb.jinqigfzy.top

[S50] C++：格式化数字
来源：http://hzp.quarkkingdee.top


<!-- 参考信息 -->