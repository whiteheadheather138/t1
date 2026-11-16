代发 wailian999

SHOW INDEX FROM users;
来源：http://ylf.9152youxi.cn

[Q73] 查看表状态
来源：http://pwk.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://noj.aibaodan.cn

[Q74] 强制使用索引
来源：http://hix.uphjek.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://igf.feifeiyinyue.top

[Q75] 日期格式化
来源：http://bst.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cck.hysaishi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gak.jyoumei.cn

[Q76] 按天统计
来源：http://dmh.jqgufenzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tbp.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://aae.jqgfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zpm.svipenyu.cn

[Q78] 当前时间
来源：http://esz.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lst.fehbvm.com

[Q79] 字符串拼接
来源：http://zlo.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://akt.ybcxt.top

[Q80] 字符串截取
来源：http://ont.uphjek.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://udm.yangfankeji.com

[Q81] 字符串替换
来源：http://ord.zhongyouzk.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://moi.sxryk.cn

[Q82] 字符长度与字节长度
来源：http://zmd.kuanghao11.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://toi.yangfankeji.com

[Q83] 大小写转换
来源：http://xtf.jyoumei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://guo.jinqigufen.top

[Q84] 去除首尾空格
来源：http://mzv.cashguo.top

SELECT TRIM(name) FROM users;
来源：http://ait.sysykeji.top

[Q85] 数值取整
来源：http://ngi.vehdjk.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://olc.hcnkem.com

[Q86] 读取 JSON 字段
来源：http://jbo.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vno.yj20258.top

[Q87] JSON 字段做条件
来源：http://dtw.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qez.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://jlg.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vvo.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://alx.xylfe.cn

[Q89] 判断表是否存在
来源：http://xhc.sweek.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xxd.chenzaomai.com

[Q90] 生成序号列
来源：http://ckm.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oah.jlsjyb.cn

================================================================================
来源：http://yqi.daxiang520.top

R. Bash 专题
来源：http://cwo.uphjek.com

================================================================================
来源：http://uih.hywenlv.cn

[R01] shebang 与严格模式
来源：http://wjm.ehwqpu.com

#!/usr/bin/env bash
来源：http://uqr.cqqwz.cn

set -euo pipefail
来源：http://jic.yanxiufei.cn

[R02] 变量赋值与使用
来源：http://rjf.haohaochexian.top

name="Tom"; echo "$name"
来源：http://qtw.yongpay.top

[R03] 只读变量
来源：http://voo.iojbl.cn

readonly PI=3.14
来源：http://xql.ybcxt.top

[R04] 位置参数
来源：http://xbx.xuetiantiany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zqs.dianchejie.cn

[R05] 参数默认值
来源：http://pua.jinghuilouyu.cn

name="${1:-default}"
来源：http://nmh.hywenlv.cn

[R06] 判断命令是否存在
来源：http://fin.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lgp.zhixingplan.top

[R07] if 判断文件
来源：http://bxr.yuanzhike.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ags.daxiang520.top

[R08] 数值比较
来源：http://obb.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://xbq.mhx1999.top

[R09] 字符串比较
来源：http://bke.0kj1m.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pey.zdqjudy.top

[R10] 正则匹配
来源：http://oqq.redwolf501.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rat.fanxiaobao.xyz

[R11] case 多分支
来源：http://irr.jinqigufen.top

case "$1" in
来源：http://alu.chenlongwang.top

start) echo "启动" ;;
来源：http://qfk.zhengqikj.top

stop)  echo "停止" ;;
来源：http://lmh.shangyingyoupin.top

*)     echo "未知命令" ;;
来源：http://zkq.iojbl.cn

esac
来源：http://qgc.zhoulong.xyz

[R12] for 遍历文件
来源：http://uln.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://ixd.xylfe.cn

[R13] for 计数循环
来源：http://hnm.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://fce.yuxming.cn

[R14] C 风格 for
来源：http://qpx.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bnk.vqdsnc.cn

[R15] while 逐行读文件
来源：http://tlf.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zam.zhixingplan.top

[R16] until 等待条件
来源：http://fib.ppjwa.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://afs.quarkkingdee.top

[R17] 数组定义与取值
来源：http://ylo.hammf.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nve.jinqigfzy.top

[R18] 遍历数组
来源：http://frt.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jvs.tianlin.xyz

[R19] 数组长度
来源：http://bkp.ywan-chungtsiang.top

echo "${#arr[@]}"
来源：http://kqy.xuanzx.com

[R20] 关联数组（字典）
来源：http://gge.jinqigufen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://avf.epnwcf.com

[R21] 字符串长度
来源：http://ote.hnqzz.top

echo "${#s}"
来源：http://gvx.guowangkeji.top

[R22] 截取子串
来源：http://tqg.pengpengdd.cyou

echo "${s:0:5}"
来源：http://ufi.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://qps.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wtc.hnqzz.top

[R24] 大小写转换
来源：http://cca.fehbvm.com

echo "${s^^}"; echo "${s,,}"
来源：http://dma.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://hpd.chenjidiqi.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://rdf.zhengqikj.top

[R26] 命令替换
来源：http://exy.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://lhc.xziqi.cn

[R27] 算术展开
来源：http://sch.shanyushiyangtech.top

echo $((1 + 2 * 3))
来源：http://zja.cucudq.cn

[R28] 浮点运算
来源：http://ouc.yvedp.cn

echo "scale=2; 10/3" | bc
来源：http://fwc.jqgfzy.top

[R29] 定义函数
来源：http://lat.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ppk.ydzc1.top

[R30] 函数返回状态码
来源：http://hoz.tanke756.top

f() { return 0; }; f || echo "失败了"
来源：http://wyg.jinqigufen.top

[R31] 局部变量
来源：http://fgu.c1oappe.top

f() { local x=1; echo "$x"; }
来源：http://ion.chenlongwang.top

[R32] 参数个数校验
来源：http://hig.ehwqpu.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wgc.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://xdt.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wig.daxiang520.top

[R34] 退出时清理
来源：http://aam.tianlin.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://tbp.ctjpmb.com

[R35] 后台执行并等待
来源：http://jyu.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://aws.daxiang520.top

[R36] 并发执行多个任务
来源：http://qwr.hywenlv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zkg.kuanghao11.cn

[R37] 把输出赋给变量
来源：http://jar.sufxvd.cn

files=$(ls -1)
来源：http://mkh.ydzc1.top

[R38] 管道串联
来源：http://ufd.yj202588.top

cat a.txt | grep -i error | wc -l
来源：http://uhs.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://yfp.quarkkingdee.top

cmd > out.log 2>&1
来源：http://gbx.sweek.top

[R40] 追加写日志
来源：http://pep.cdnleiting.top

echo "log" >> out.log
来源：http://jvw.sysykeji.top

[R41] 丢弃输出
来源：http://rdi.aizwys.cn

cmd >/dev/null 2>&1
来源：http://dve.xylfe.cn

[R42] 输入重定向
来源：http://dte.ivvv.top

wc -l < a.txt
来源：http://nnl.sweek.top

[R43] 按名字查找文件
来源：http://vwj.andypj.xyz

find . -name "*.log" -type f
来源：http://iae.chenlongwang.top

[R44] 按修改时间查找
来源：http://knm.ydzc1.top

find . -mtime -7 -type f
来源：http://taa.zhengqikj.top

[R45] 批量删除
来源：http://ulj.shangyingyoupin.top

find . -name "*.tmp" -delete
来源：http://uri.iojbl.cn

[R46] 递归替换文件内容
来源：http://fce.snrcjt.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vsg.0kj1m.cn

[R47] sed 单行替换
来源：http://fnd.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://olk.jinqigfzy.top

[R48] awk 取指定列
来源：http://pag.shzxlz.cn

awk '{print $1, $3}' a.txt
来源：http://lhr.shanyushiyangtech.top

[R49] awk 带条件
来源：http://imc.yonumen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ozr.cashguo.top

[R50] awk 求和
来源：http://ptz.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yyo.tianlin.xyz

[R51] 排序去重取前几
来源：http://xhi.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://tht.hongshengwenyu.top

[R52] 统计行数
来源：http://lmo.mhx1999.top

wc -l a.txt
来源：http://brh.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://dpp.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yga.aizwys.cn

[R54] 比较两个文件
来源：http://zvo.gaohongyu789.top

diff a.txt b.txt
来源：http://jgx.xziqi.cn

[R55] 压缩与解压
来源：http://bsm.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mce.shzxlz.cn

[R56] 远程拷贝
来源：http://tgr.yuanzhike.top

scp file user@host:/path/
来源：http://bdt.yuanzhike.top

[R57] 远程执行命令
来源：http://tcp.bbcook.cn

ssh user@host 'uptime'
来源：http://ret.yueranfly.top

[R58] 下载文件
来源：http://vqe.9152youxi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mln.mhx1999.top

[R59] 发 POST JSON
来源：http://agk.xziqi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nyk.xinyue.icu

[R60] 只看 HTTP 状态码
来源：http://xkb.sjlbkw.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vve.jinqigfzy.top

[R61] 磁盘占用
来源：http://cod.zhijiandao.cn

df -h;  du -sh *
来源：http://wbe.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://xpa.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://ljo.birdmap.top

[R63] 内存与进程
来源：http://bbb.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://ajr.ybcxt.top

[R64] 结束进程
来源：http://uty.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://hvx.chenjidiqi.icu

[R65] 查看端口占用
来源：http://dvm.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ptk.guannengcc.top

[R66] 定时任务
来源：http://oeo.ydzc1.top

crontab -e;  crontab -l
来源：http://oii.52xcode.cn

[R67] 生成随机十六进制串
来源：http://vng.chenzaomai.com

openssl rand -hex 16
来源：http://frn.jlsjyb.cn

[R68] 计算文件校验值
来源：http://xhi.pycfn.com

sha256sum a.txt;  md5sum a.txt
来源：http://thz.9152youxi.cn

[R69] 生成随机密码
来源：http://lxg.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://bkx.cucudq.cn

[R70] 时间戳与互转
来源：http://jay.yj20258.top

date +%s;  date -d @1700000000
来源：http://xex.hongshengwenyu.top

[R71] 日期格式化
来源：http://cit.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gcu.sufxvd.cn

[R72] 等待端口就绪
来源：http://dth.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dpi.xuetiantiany.cn

[R73] 分割大日志
来源：http://vdm.zhongyouzk.top

split -l 1000 big.log part_
来源：http://ybr.wangshuangyany.cn

[R74] 批量重命名
来源：http://aso.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kra.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://dkv.jqgufenzy.top

export PATH="$HOME/bin:$PATH"
来源：http://vgk.ydjk.org.cn

[R76] 使用临时文件
来源：http://tqe.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://djo.shuidangran.top

[R77] 读取用户输入
来源：http://gqj.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://har.xylfe.cn

[R78] 交互式菜单
来源：http://jxf.ydzc1.top

select opt in a b c; do echo "$opt"; break; done
来源：http://got.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://pky.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oqv.hfpthk.cn

[R80] 查看脚本执行耗时
来源：http://lng.chenlongwang.top

time ./run.sh
来源：http://lni.zdqjudy.top

================================================================================
来源：http://rwr.jianghu66.top

S. C / C++ 专题
来源：http://uvp.smart0.xyz

================================================================================
来源：http://yzd.xziqi.cn

[S01] C：Hello World
来源：http://cxm.mhx1999.top

#include <stdio.h>
来源：http://xhh.xuetiantiany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xhn.zdbjq.cn

[S02] C：变量与格式化输出
来源：http://xat.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://gpl.yongpay.top

[S03] C：读入整数
来源：http://hqd.nwbrower.top

int x; scanf("%d", &x);
来源：http://ecz.jqgfzy.top

[S04] C：字符串复制
来源：http://ptj.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tdf.yueranfly.top

[S05] C：字符串长度
来源：http://ssp.9152youxi.cn

strlen(s)
来源：http://wal.kuanghao11.cn

[S06] C：字符串比较
来源：http://umg.bjfxy.top

strcmp(a, b) == 0
来源：http://fop.9152youxi.cn

[S07] C：数组遍历求和
来源：http://mbq.daxiang520.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uvd.fanxiaobao.xyz

[S08] C：动态内存分配与释放
来源：http://dev.andypj.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dxc.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://zoq.andypj.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rzt.c1oappe.top

[S10] C：指针与解引用
来源：http://myl.hnqzz.top

int *p = &a;  *p = 5;
来源：http://vyb.yonumen.top

[S11] C：逐行读文件
来源：http://kmk.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://tui.wangshuangyany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kpu.jiagoushi.top

fclose(f);
来源：http://qpz.tian-w.cn

[S12] C：写文件
来源：http://lly.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xmi.aizwys.cn

[S13] C：宏定义
来源：http://njs.birdmap.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wzo.yongpay.top

[S14] C：枚举
来源：http://sbm.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://sqt.hcnkem.com

[S15] C：类型转换
来源：http://vil.iojbl.cn

(double) a / b
来源：http://xlg.hammf.cn

[S16] C：位操作置位
来源：http://jwm.hfpthk.cn

x |= (1 << 3);
来源：http://ocq.yj20258888.top

[S17] C：安全拼接字符串
来源：http://bcf.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ktt.shuidangran.top

[S18] C：命令行参数
来源：http://zfy.zycfv.cn

int main(int argc, char **argv)
来源：http://ggc.redwolf501.top

[S19] C：快速排序
来源：http://bdc.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tvk.zhengqikj.top

[S20] C：二分查找
来源：http://krp.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://avx.yonumen.top

[S21] C：字符类别判断
来源：http://suw.kuanghao11.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://csg.fengsongda.top

[S22] C：字符串转数字
来源：http://dql.xinyue.icu

atoi("42");  strtod("3.14", NULL);
来源：http://cft.cucudq.cn

[S23] C：随机数
来源：http://bxs.nanxuanxn.top

srand(time(NULL));  int r = rand() % 100;
来源：http://aaw.yj202588.top

[S24] C：获取本地时间
来源：http://qgd.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gnx.jianghu66.top

[S25] C：内存拷贝
来源：http://kfa.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://xdz.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://djl.ivvv.top

memset(a, 0, sizeof a);
来源：http://lrf.xuetiantiany.cn

[S27] C：定义常量
来源：http://kbg.uphjek.com

const double PI = 3.14159;
来源：http://hgk.hywenlv.cn

[S28] C：静态变量
来源：http://hqg.havefunace.top

static int counter = 0;
来源：http://gey.uphjek.com

[S29] C：变参函数
来源：http://sft.zhijiandao.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jss.nanxuanxn.top

[S30] C：头文件保护
来源：http://toq.jqgfzy.top

#ifndef X_H
来源：http://cpw.dashuyun.cn

#define X_H
来源：http://zkx.jqgufenzy.top

#endif
来源：http://cyv.cheryme.top

[S31] C++：Hello World
来源：http://nmk.wangshuangyany.cn

#include <iostream>
来源：http://eyd.hnqzz.top

int main() { std::cout << "Hello\n"; }
来源：http://bgf.havefunace.top

[S32] C++：字符串
来源：http://vmo.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://tqj.gaohongyu789.top

[S33] C++：vector 增删
来源：http://kwk.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://psl.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://hpx.fehbvm.com

for (auto &x : v) { std::cout << x; }
来源：http://mse.cashguo.top

[S35] C++：map
来源：http://kdg.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://slt.cucudq.cn

[S36] C++：unordered_map
来源：http://rbv.snrcjt.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uic.jyoumei.cn

[S37] C++：set
来源：http://hyd.hcnkem.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gtm.pycfn.com

[S38] C++：排序
来源：http://lwk.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://lrb.xylfe.cn

[S39] C++：自定义比较器排序
来源：http://klj.cdnleiting.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nwe.hongshengwenyu.top

[S40] C++：查找元素
来源：http://bwt.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zpl.shuidangran.top

[S41] C++：类与构造函数
来源：http://xbn.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://guv.nwbrower.top

[S42] C++：继承与虚函数
来源：http://iur.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://neg.zdqjudy.top


<!-- 参考信息 -->