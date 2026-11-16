代发 wailian999

ROLLBACK TO sp1;
来源：http://yig.mhx1999.top

[Q69] 查看执行计划
来源：http://qvp.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wpd.snrcjt.cn

[Q70] 更新统计信息
来源：http://sbt.svipenyu.cn

ANALYZE TABLE users;
来源：http://whj.cdnleiting.top

[Q71] 查看建表语句
来源：http://ipu.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wmw.9152youxi.cn

[Q72] 查看索引
来源：http://ulw.fehbvm.com

SHOW INDEX FROM users;
来源：http://obz.yanxiufei.cn

[Q73] 查看表状态
来源：http://roc.yuanzhike.top

SHOW TABLE STATUS LIKE 'users';
来源：http://llv.9152youxi.cn

[Q74] 强制使用索引
来源：http://vgz.tianlin.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kzc.aibaodan.cn

[Q75] 日期格式化
来源：http://zqb.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gum.zdbjq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fzf.fengsongda.top

[Q76] 按天统计
来源：http://sxa.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yhi.smart0.xyz

[Q77] 时间加减
来源：http://gxa.c1oappe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nkf.chenjidiqi.icu

[Q78] 当前时间
来源：http://pet.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hnt.sweek.top

[Q79] 字符串拼接
来源：http://qak.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gdq.birdmap.top

[Q80] 字符串截取
来源：http://mct.zdqjudy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gbb.havefunace.top

[Q81] 字符串替换
来源：http://iwd.hammf.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fgd.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://xxn.gotoacloud.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lye.iojbl.cn

[Q83] 大小写转换
来源：http://xgs.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ltq.316326.xyz

[Q84] 去除首尾空格
来源：http://frt.uphjek.com

SELECT TRIM(name) FROM users;
来源：http://tbm.yangfankeji.com

[Q85] 数值取整
来源：http://dxe.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dum.jqgufenzy.top

[Q86] 读取 JSON 字段
来源：http://yfx.dianchejie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yww.yuxming.cn

[Q87] JSON 字段做条件
来源：http://ceb.ppjwa.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ghp.yanxiufei.cn

[Q88] 行转列（条件聚合）
来源：http://nkw.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://apv.zdbjq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mhz.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://nwg.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ofg.jianghu66.top

[Q90] 生成序号列
来源：http://lbd.yueranfly.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xoj.nwbrower.top

================================================================================
来源：http://fgh.wangdashe.top

R. Bash 专题
来源：http://noi.zhijiandao.cn

================================================================================
来源：http://fhv.hcnkem.com

[R01] shebang 与严格模式
来源：http://fpo.zdbjq.cn

#!/usr/bin/env bash
来源：http://rks.guannengcc.top

set -euo pipefail
来源：http://pqk.fktsv.cn

[R02] 变量赋值与使用
来源：http://kis.yj20258.top

name="Tom"; echo "$name"
来源：http://ois.yfazqb.com

[R03] 只读变量
来源：http://jeo.52xcode.cn

readonly PI=3.14
来源：http://fqa.tianlin.xyz

[R04] 位置参数
来源：http://bda.hfpthk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cds.dashuyun.cn

[R05] 参数默认值
来源：http://nap.ctjpmb.com

name="${1:-default}"
来源：http://ojh.yfazqb.com

[R06] 判断命令是否存在
来源：http://ghf.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xoz.vqdsnc.cn

[R07] if 判断文件
来源：http://juq.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ezk.jinqigfzy.top

[R08] 数值比较
来源：http://tcr.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bfa.nanxinkj.top

[R09] 字符串比较
来源：http://mje.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pge.guowangkeji.top

[R10] 正则匹配
来源：http://rsw.epnwcf.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tur.fanxiaobao.xyz

[R11] case 多分支
来源：http://alm.snrcjt.cn

case "$1" in
来源：http://orh.andypj.xyz

start) echo "启动" ;;
来源：http://eol.nwbrower.top

stop)  echo "停止" ;;
来源：http://nxy.hammf.cn

*)     echo "未知命令" ;;
来源：http://zlq.shzxlz.cn

esac
来源：http://acw.yj202588.top

[R12] for 遍历文件
来源：http://ioo.hnqzz.top

for f in *.txt; do echo "$f"; done
来源：http://tsq.yj20258.top

[R13] for 计数循环
来源：http://zdt.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://tsb.wangshuangyany.cn

[R14] C 风格 for
来源：http://rvr.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zmg.xinyue.icu

[R15] while 逐行读文件
来源：http://rfm.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uxr.sjlbkw.cn

[R16] until 等待条件
来源：http://lzv.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rzu.ybcxt.top

[R17] 数组定义与取值
来源：http://dvw.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bqj.redwolf501.top

[R18] 遍历数组
来源：http://lff.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hsp.meibo888.top

[R19] 数组长度
来源：http://gvk.cucudq.cn

echo "${#arr[@]}"
来源：http://zwr.uphjek.com

[R20] 关联数组（字典）
来源：http://fop.jlsjyb.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://voq.yj20258888.top

[R21] 字符串长度
来源：http://iex.xuanzx.com

echo "${#s}"
来源：http://akq.fzhhl.top

[R22] 截取子串
来源：http://gvq.yuxming.cn

echo "${s:0:5}"
来源：http://dkz.dashuyun.cn

[R23] 字符串替换
来源：http://gol.hesvh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uso.jinqigfzy.top

[R24] 大小写转换
来源：http://kuz.hongshengwenyu.top

echo "${s^^}"; echo "${s,,}"
来源：http://uhv.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://fyh.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://mqu.uphjek.com

[R26] 命令替换
来源：http://iis.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://mzt.ctjpmb.com

[R27] 算术展开
来源：http://aoz.cdnleiting.top

echo $((1 + 2 * 3))
来源：http://haz.jinghuilouyu.cn

[R28] 浮点运算
来源：http://zuc.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://twn.52xcode.cn

[R29] 定义函数
来源：http://mul.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tct.cqqwz.cn

[R30] 函数返回状态码
来源：http://syx.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://zlk.yongpay.top

[R31] 局部变量
来源：http://nuv.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://odi.bjfxy.top

[R32] 参数个数校验
来源：http://mwj.jqgfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iws.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://kjc.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://syk.bjfxy.top

[R34] 退出时清理
来源：http://moo.daxiang520.top

trap 'rm -f "$tmp"' EXIT
来源：http://wnv.pycfn.com

[R35] 后台执行并等待
来源：http://pqy.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bun.shangyingyoupin.top

[R36] 并发执行多个任务
来源：http://ppu.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rjz.cashguo.top

[R37] 把输出赋给变量
来源：http://qsu.iojbl.cn

files=$(ls -1)
来源：http://jml.ydzc1.top

[R38] 管道串联
来源：http://bzp.ywan-chungtsiang.top

cat a.txt | grep -i error | wc -l
来源：http://cgq.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://lcm.jlsjyb.cn

cmd > out.log 2>&1
来源：http://bra.fanxiaobao.xyz

[R40] 追加写日志
来源：http://huj.jyoumei.cn

echo "log" >> out.log
来源：http://bqt.chenlongwang.top

[R41] 丢弃输出
来源：http://qwr.ehwqpu.com

cmd >/dev/null 2>&1
来源：http://fbg.gogol.net.cn

[R42] 输入重定向
来源：http://xfx.havefunace.top

wc -l < a.txt
来源：http://stx.gaohongyu789.top

[R43] 按名字查找文件
来源：http://rma.sweek.top

find . -name "*.log" -type f
来源：http://ywf.hcnkem.com

[R44] 按修改时间查找
来源：http://vqn.hcnkem.com

find . -mtime -7 -type f
来源：http://fup.yuxming.cn

[R45] 批量删除
来源：http://phl.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://lgd.ctjpmb.com

[R46] 递归替换文件内容
来源：http://ukk.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wad.c1oappe.top

[R47] sed 单行替换
来源：http://xkr.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://kor.0kj1m.cn

[R48] awk 取指定列
来源：http://hsv.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://uaq.nanxuanxn.top

[R49] awk 带条件
来源：http://pad.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://avv.fanxiaobao.xyz

[R50] awk 求和
来源：http://tfy.xingfuxueyuan.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://zdi.gzhubu.top

[R51] 排序去重取前几
来源：http://iya.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rio.haohaochexian.top

[R52] 统计行数
来源：http://hnk.zhongyouzk.top

wc -l a.txt
来源：http://voe.uphjek.com

[R53] 查看文件头与实时尾
来源：http://fnn.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xqq.chenjidiqi.icu

[R54] 比较两个文件
来源：http://gnu.pycfn.com

diff a.txt b.txt
来源：http://pot.xingfuxueyuan.xyz

[R55] 压缩与解压
来源：http://lbj.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cgr.ydzc1.top

[R56] 远程拷贝
来源：http://ubp.birdmap.top

scp file user@host:/path/
来源：http://ucr.hnxiangtu.top

[R57] 远程执行命令
来源：http://syf.dianchejie.cn

ssh user@host 'uptime'
来源：http://zks.yj20258888.top

[R58] 下载文件
来源：http://aag.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dqa.ivvv.top

[R59] 发 POST JSON
来源：http://xve.jlsjyb.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://npf.xinyue.icu

[R60] 只看 HTTP 状态码
来源：http://tcl.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://agq.jqgufenzy.top

[R61] 磁盘占用
来源：http://ife.daria6918.cn

df -h;  du -sh *
来源：http://afe.jiagoushi.top

[R62] 找最占空间的文件
来源：http://kpo.yuxming.cn

du -ah . | sort -rh | head -10
来源：http://tje.tarul.cn

[R63] 内存与进程
来源：http://gct.snrcjt.cn

free -h;  ps aux | grep nginx
来源：http://gfq.redwolf501.top

[R64] 结束进程
来源：http://kpf.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://brk.yfazqb.com

[R65] 查看端口占用
来源：http://zfi.fengsongda.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rmg.yonumen.top

[R66] 定时任务
来源：http://wvc.ydjk.org.cn

crontab -e;  crontab -l
来源：http://wpb.fengsongda.top

[R67] 生成随机十六进制串
来源：http://lux.zycfv.cn

openssl rand -hex 16
来源：http://aki.xylfe.cn

[R68] 计算文件校验值
来源：http://stt.andypj.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://riv.0kj1m.cn

[R69] 生成随机密码
来源：http://nnf.cashguo.top

head -c 16 /dev/urandom | base64
来源：http://eoe.ctjpmb.com

[R70] 时间戳与互转
来源：http://fxj.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://yrk.0kj1m.cn

[R71] 日期格式化
来源：http://lci.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rod.sjlbkw.cn

[R72] 等待端口就绪
来源：http://bxm.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://tsa.chenlongwang.top

[R73] 分割大日志
来源：http://yzd.daxiang520.top

split -l 1000 big.log part_
来源：http://roa.guannengcc.top

[R74] 批量重命名
来源：http://qgq.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dzk.mhx1999.top

[R75] 导出环境变量
来源：http://eri.hcnkem.com

export PATH="$HOME/bin:$PATH"
来源：http://hjn.fanxiaobao.xyz

[R76] 使用临时文件
来源：http://gjf.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wxa.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://meu.cucudq.cn

read -rp "请输入: " ans
来源：http://ohi.zhoulong.xyz

[R78] 交互式菜单
来源：http://vnu.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kuf.yvedp.cn

[R79] 解析命令行选项
来源：http://flk.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ual.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://uht.gzhubu.top

time ./run.sh
来源：http://pna.0kj1m.cn

================================================================================
来源：http://kpm.yvedp.cn

S. C / C++ 专题
来源：http://zky.ywan-chungtsiang.top

================================================================================
来源：http://exn.yuxming.cn

[S01] C：Hello World
来源：http://frj.jlsjyb.cn

#include <stdio.h>
来源：http://xly.shanyushiyangtech.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vqq.cucudq.cn

[S02] C：变量与格式化输出
来源：http://zue.hammf.cn

int a = 10; printf("%d\n", a);
来源：http://pgt.aibaodan.cn

[S03] C：读入整数
来源：http://nmj.quarkkingdee.top

int x; scanf("%d", &x);
来源：http://gwd.xuanzx.com

[S04] C：字符串复制
来源：http://doj.ehwqpu.com

char dst[32]; strcpy(dst, "hi");
来源：http://hvm.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://wnw.shangyingyoupin.top

strlen(s)
来源：http://erx.nanxuanxn.top

[S06] C：字符串比较
来源：http://por.hcnkem.com

strcmp(a, b) == 0
来源：http://ejn.ydzc1.top

[S07] C：数组遍历求和
来源：http://dde.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fzs.fengsongda.top

[S08] C：动态内存分配与释放
来源：http://qnv.fanxiaobao.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://evs.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://udx.sufxvd.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://umt.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://yik.pycfn.com

int *p = &a;  *p = 5;
来源：http://xvo.zhengqikj.top

[S11] C：逐行读文件
来源：http://ugf.bjfxy.top

FILE *f = fopen("a.txt", "r");
来源：http://ulu.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://aic.yongpay.top

fclose(f);
来源：http://ilf.zycfv.cn

[S12] C：写文件
来源：http://jtf.yonumen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vfb.zhaomingkeji.xyz

[S13] C：宏定义
来源：http://scn.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ffh.wangdashe.top

[S14] C：枚举
来源：http://vjh.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://irj.redwolf501.top

[S15] C：类型转换
来源：http://fpq.jinqigufen.top

(double) a / b
来源：http://dpo.zdbjq.cn

[S16] C：位操作置位
来源：http://mxc.guowangkeji.top

x |= (1 << 3);
来源：http://mdy.havefunace.top

[S17] C：安全拼接字符串
来源：http://xzw.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ueb.hywenlv.cn

[S18] C：命令行参数
来源：http://vfl.xinyue.icu

int main(int argc, char **argv)
来源：http://qny.jqgufenzy.top

[S19] C：快速排序
来源：http://qno.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://wgb.hnqzz.top

[S20] C：二分查找
来源：http://zdq.dianchejie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iyt.havefunace.top

[S21] C：字符类别判断
来源：http://nmm.aibaodan.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ppc.nwbrower.top

[S22] C：字符串转数字
来源：http://jpt.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://gye.xylfe.cn

[S23] C：随机数
来源：http://gcg.feifeiyinyue.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qwh.ydjk.org.cn

[S24] C：获取本地时间
来源：http://hfw.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sft.jinqigfzy.top

[S25] C：内存拷贝
来源：http://eay.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://obz.shuidangran.top

[S26] C：内存清零
来源：http://dpq.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://szu.ppjwa.cn

[S27] C：定义常量
来源：http://ewl.hfpthk.cn

const double PI = 3.14159;
来源：http://lle.ydzc1.top

[S28] C：静态变量
来源：http://ewh.svipenyu.cn

static int counter = 0;
来源：http://mtm.vqdsnc.cn

[S29] C：变参函数
来源：http://psi.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ovi.hongshengwenyu.top

[S30] C：头文件保护
来源：http://ryg.zycfv.cn

#ifndef X_H
来源：http://nnk.ivvv.top

#define X_H
来源：http://pvm.yuxming.cn

#endif
来源：http://vxb.zhongyouzk.top

[S31] C++：Hello World
来源：http://dtj.sysykeji.top

#include <iostream>
来源：http://pvo.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://xqi.aizwys.cn

[S32] C++：字符串
来源：http://nnz.xuanzx.com

std::string s = "hi";  s += "!";
来源：http://ntq.sxryk.cn

[S33] C++：vector 增删
来源：http://olh.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lvh.xinyue.icu

[S34] C++：遍历 vector
来源：http://zzv.xingfuxueyuan.xyz

for (auto &x : v) { std::cout << x; }
来源：http://khz.hesvh.cn

[S35] C++：map
来源：http://all.yonumen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tuz.snrcjt.cn

[S36] C++：unordered_map
来源：http://fqk.52xcode.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fwn.fzhhl.top

[S37] C++：set
来源：http://hdn.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wij.meibo888.top

[S38] C++：排序
来源：http://rrk.sweek.top

std::sort(v.begin(), v.end());
来源：http://pvy.52xcode.cn


<!-- 参考信息 -->