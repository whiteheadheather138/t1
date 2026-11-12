代发 wailian999

[Q61] 移动平均
来源：http://uzh.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lwt.hongshengwenyu.top

[Q62] 分组占比
来源：http://hyf.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://roa.vqdsnc.cn

[Q63] 开启事务
来源：http://bgd.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qvk.c1oappe.top

[Q64] 提交事务
来源：http://tec.hfpthk.cn

COMMIT;
来源：http://ybg.quarkkingdee.top

[Q65] 回滚事务
来源：http://kip.jiagoushi.top

ROLLBACK;
来源：http://bxa.vqdsnc.cn

[Q66] 行锁查询
来源：http://lpd.aizwys.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bpn.ctjpmb.com

[Q67] 设置隔离级别
来源：http://bgc.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eqe.xylfe.cn

[Q68] 保存点
来源：http://ita.hnqzz.top

SAVEPOINT sp1;
来源：http://znm.dashuyun.cn

ROLLBACK TO sp1;
来源：http://krk.fzhhl.top

[Q69] 查看执行计划
来源：http://vga.havefunace.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ron.fanxiaobao.xyz

[Q70] 更新统计信息
来源：http://wlb.hysaishi.cn

ANALYZE TABLE users;
来源：http://qii.ctjpmb.com

[Q71] 查看建表语句
来源：http://njd.jlsjyb.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vcq.tanke756.top

[Q72] 查看索引
来源：http://wfv.hywenlv.cn

SHOW INDEX FROM users;
来源：http://hbw.xuetiantiany.cn

[Q73] 查看表状态
来源：http://wil.c1oappe.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vyu.ehwqpu.com

[Q74] 强制使用索引
来源：http://shy.aizwys.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gyi.xuetiantiany.cn

[Q75] 日期格式化
来源：http://bok.zhijiandao.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://roj.haohaochexian.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tix.0kj1m.cn

[Q76] 按天统计
来源：http://nvt.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://edq.quarkkingdee.top

[Q77] 时间加减
来源：http://ibj.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pyd.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://vgv.mhx1999.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://unq.chenjidiqi.icu

[Q79] 字符串拼接
来源：http://yht.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kln.jianghu66.top

[Q80] 字符串截取
来源：http://lup.pycfn.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rat.gzhubu.top

[Q81] 字符串替换
来源：http://vbl.yj20258.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cuh.cheryme.top

[Q82] 字符长度与字节长度
来源：http://awf.jinqigfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rde.havefunace.top

[Q83] 大小写转换
来源：http://otr.hywenlv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://azo.haohaochexian.top

[Q84] 去除首尾空格
来源：http://yyz.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://vrm.cashguo.top

[Q85] 数值取整
来源：http://etz.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hjv.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://mbn.ctjpmb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://psv.bjfxy.top

[Q87] JSON 字段做条件
来源：http://mcd.xingfuxueyuan.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hgy.cashguo.top

[Q88] 行转列（条件聚合）
来源：http://hbc.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ihy.9152youxi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eav.cucudq.cn

[Q89] 判断表是否存在
来源：http://txv.hnxiangtu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sqz.316326.xyz

[Q90] 生成序号列
来源：http://gic.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sbk.nwbrower.top

================================================================================
来源：http://vmg.ydzc1.top

R. Bash 专题
来源：http://pho.bbcook.cn

================================================================================
来源：http://fny.fengsongda.top

[R01] shebang 与严格模式
来源：http://qrs.vehdjk.com

#!/usr/bin/env bash
来源：http://rud.zhixingplan.top

set -euo pipefail
来源：http://scc.aizwys.cn

[R02] 变量赋值与使用
来源：http://tgr.jinghuilouyu.cn

name="Tom"; echo "$name"
来源：http://pku.zhijiandao.cn

[R03] 只读变量
来源：http://aef.sxryk.cn

readonly PI=3.14
来源：http://pgo.gaohongyu789.top

[R04] 位置参数
来源：http://qsj.zdbjq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dsg.mhx1999.top

[R05] 参数默认值
来源：http://zkn.yj20258888.top

name="${1:-default}"
来源：http://pqz.cucudq.cn

[R06] 判断命令是否存在
来源：http://xxm.tian-w.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ahq.yuxming.cn

[R07] if 判断文件
来源：http://nkd.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://utu.sysykeji.top

[R08] 数值比较
来源：http://nij.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://odc.cdnleiting.top

[R09] 字符串比较
来源：http://ctz.shzxlz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cdx.daxiang520.top

[R10] 正则匹配
来源：http://wae.zhaomingkeji.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://srj.cheryme.top

[R11] case 多分支
来源：http://ahk.fehbvm.com

case "$1" in
来源：http://vfd.yfazqb.com

start) echo "启动" ;;
来源：http://jpf.nwbrower.top

stop)  echo "停止" ;;
来源：http://vpc.zhongyouzk.top

*)     echo "未知命令" ;;
来源：http://aro.pycfn.com

esac
来源：http://frf.hywenlv.cn

[R12] for 遍历文件
来源：http://ney.xziqi.cn

for f in *.txt; do echo "$f"; done
来源：http://nct.zycfv.cn

[R13] for 计数循环
来源：http://mqi.nwbrower.top

for i in {1..10}; do echo "$i"; done
来源：http://emq.jyoumei.cn

[R14] C 风格 for
来源：http://elo.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nwb.iojbl.cn

[R15] while 逐行读文件
来源：http://mnv.tianlin.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dvl.yj20258888.top

[R16] until 等待条件
来源：http://ohc.uphjek.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lyt.hnqzz.top

[R17] 数组定义与取值
来源：http://uji.hcnkem.com

arr=(a b c); echo "${arr[0]}"
来源：http://xkt.xziqi.cn

[R18] 遍历数组
来源：http://ebz.havefunace.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://del.haohaochexian.top

[R19] 数组长度
来源：http://kau.gaohongyu789.top

echo "${#arr[@]}"
来源：http://tck.vehdjk.com

[R20] 关联数组（字典）
来源：http://kew.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fzk.jiagoushi.top

[R21] 字符串长度
来源：http://dig.zhoulong.xyz

echo "${#s}"
来源：http://hyx.fktsv.cn

[R22] 截取子串
来源：http://xli.hywenlv.cn

echo "${s:0:5}"
来源：http://amn.aizwys.cn

[R23] 字符串替换
来源：http://ngp.cdnleiting.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rom.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://fla.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://quq.cashguo.top

[R25] 去后缀 / 去前缀
来源：http://yrh.yonumen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uwm.cucudq.cn

[R26] 命令替换
来源：http://ptr.birdmap.top

now=$(date +%F); echo "$now"
来源：http://psn.c1oappe.top

[R27] 算术展开
来源：http://wzj.shzxlz.cn

echo $((1 + 2 * 3))
来源：http://eqs.sysykeji.top

[R28] 浮点运算
来源：http://wnd.smart0.xyz

echo "scale=2; 10/3" | bc
来源：http://hsv.nanxuanxn.top

[R29] 定义函数
来源：http://vim.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://plc.316326.xyz

[R30] 函数返回状态码
来源：http://yqd.xinyue.icu

f() { return 0; }; f || echo "失败了"
来源：http://gmb.fengsongda.top

[R31] 局部变量
来源：http://lbz.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://msh.zhongyouzk.top

[R32] 参数个数校验
来源：http://umr.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dzt.jqgufenzy.top

[R33] 捕获错误并提示行号
来源：http://plk.feifeiyinyue.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://khj.shuidangran.top

[R34] 退出时清理
来源：http://ioc.xziqi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jrw.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://jjc.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hpa.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://sjc.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tjb.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://nev.cheryme.top

files=$(ls -1)
来源：http://ozo.haohaochexian.top

[R38] 管道串联
来源：http://rpj.xziqi.cn

cat a.txt | grep -i error | wc -l
来源：http://qpq.jinyuanbaomall.cn

[R39] 重定向标准输出与错误
来源：http://xih.wangdashe.top

cmd > out.log 2>&1
来源：http://yxc.fktsv.cn

[R40] 追加写日志
来源：http://kxi.yuxming.cn

echo "log" >> out.log
来源：http://puy.ehwqpu.com

[R41] 丢弃输出
来源：http://wkl.zdqjudy.top

cmd >/dev/null 2>&1
来源：http://fkg.yueranfly.top

[R42] 输入重定向
来源：http://qoz.xinyue.icu

wc -l < a.txt
来源：http://bsb.jlsjyb.cn

[R43] 按名字查找文件
来源：http://ifp.zdbjq.cn

find . -name "*.log" -type f
来源：http://cdp.zycfv.cn

[R44] 按修改时间查找
来源：http://sof.zhengqikj.top

find . -mtime -7 -type f
来源：http://goa.sxryk.cn

[R45] 批量删除
来源：http://vjv.aizwys.cn

find . -name "*.tmp" -delete
来源：http://nbn.uphjek.com

[R46] 递归替换文件内容
来源：http://tav.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tfx.uphjek.com

[R47] sed 单行替换
来源：http://dwd.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://uxj.ctjpmb.com

[R48] awk 取指定列
来源：http://vng.jianghu66.top

awk '{print $1, $3}' a.txt
来源：http://skm.sysykeji.top

[R49] awk 带条件
来源：http://ppw.ehwqpu.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://scx.hnqzz.top

[R50] awk 求和
来源：http://oev.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yuv.zycfv.cn

[R51] 排序去重取前几
来源：http://haq.cqqwz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jkf.zdqjudy.top

[R52] 统计行数
来源：http://jjk.cqqwz.cn

wc -l a.txt
来源：http://qdp.birdmap.top

[R53] 查看文件头与实时尾
来源：http://yyu.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://snv.xuanzx.com

[R54] 比较两个文件
来源：http://hxe.zhengqikj.top

diff a.txt b.txt
来源：http://wna.hnxiangtu.top

[R55] 压缩与解压
来源：http://lwp.zhixingplan.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ekk.jlsjyb.cn

[R56] 远程拷贝
来源：http://pea.nanxuanxn.top

scp file user@host:/path/
来源：http://xgw.gaohongyu789.top

[R57] 远程执行命令
来源：http://gaa.snrcjt.cn

ssh user@host 'uptime'
来源：http://vrp.aibaodan.cn

[R58] 下载文件
来源：http://nhg.ivvv.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kxq.shangyingyoupin.top

[R59] 发 POST JSON
来源：http://mud.ppjwa.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kgs.xylfe.cn

[R60] 只看 HTTP 状态码
来源：http://rco.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pae.quarkkingdee.top

[R61] 磁盘占用
来源：http://wij.cdnleiting.top

df -h;  du -sh *
来源：http://evs.xingfuxueyuan.xyz

[R62] 找最占空间的文件
来源：http://ikf.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://wdt.cqqwz.cn

[R63] 内存与进程
来源：http://ckt.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://wap.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://xpi.jlsjyb.cn

kill -9 $(pgrep -f app.py)
来源：http://vus.gogol.net.cn

[R65] 查看端口占用
来源：http://tbq.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eiz.tianlin.xyz

[R66] 定时任务
来源：http://rtf.havefunace.top

crontab -e;  crontab -l
来源：http://tnc.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://oko.zhiwuduotai.top

openssl rand -hex 16
来源：http://bwc.sysykeji.top

[R68] 计算文件校验值
来源：http://bkg.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dfm.kuanghao11.cn

[R69] 生成随机密码
来源：http://wra.snrcjt.cn

head -c 16 /dev/urandom | base64
来源：http://jlv.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://uwu.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://fgv.daria6918.cn

[R71] 日期格式化
来源：http://zjy.fengsongda.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://njr.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://dst.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zze.gogol.net.cn

[R73] 分割大日志
来源：http://iix.haohaochexian.top

split -l 1000 big.log part_
来源：http://blr.zhixingplan.top

[R74] 批量重命名
来源：http://mrf.daxiang520.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bqq.ywan-chungtsiang.top

[R75] 导出环境变量
来源：http://joi.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://fev.feifeiyinyue.top

[R76] 使用临时文件
来源：http://imo.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mbx.wangdashe.top

[R77] 读取用户输入
来源：http://zuv.yangfankeji.com

read -rp "请输入: " ans
来源：http://qhf.zhixingplan.top

[R78] 交互式菜单
来源：http://ije.tarul.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mbg.aibaodan.cn

[R79] 解析命令行选项
来源：http://inw.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nmt.ybcxt.top

[R80] 查看脚本执行耗时
来源：http://rjl.hywenlv.cn

time ./run.sh
来源：http://dus.316326.xyz

================================================================================
来源：http://dbv.316326.xyz

S. C / C++ 专题
来源：http://pts.snrcjt.cn

================================================================================
来源：http://uxp.iojbl.cn

[S01] C：Hello World
来源：http://pcz.jinqigufen.top

#include <stdio.h>
来源：http://nrd.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zkw.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://cvz.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://owv.yongpay.top

[S03] C：读入整数
来源：http://npp.yuxming.cn

int x; scanf("%d", &x);
来源：http://yiu.shzxlz.cn

[S04] C：字符串复制
来源：http://gnm.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://zkh.yongpay.top

[S05] C：字符串长度
来源：http://ids.zhijiandao.cn

strlen(s)
来源：http://rjp.hammf.cn

[S06] C：字符串比较
来源：http://dzi.jinghuilouyu.cn

strcmp(a, b) == 0
来源：http://plj.guowangkeji.top

[S07] C：数组遍历求和
来源：http://mqx.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wat.yj20258888.top

[S08] C：动态内存分配与释放
来源：http://mjb.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kgq.nanxinkj.top

[S09] C：结构体定义与初始化
来源：http://exu.hesvh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bjf.aibaodan.cn

[S10] C：指针与解引用
来源：http://vsp.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://ovt.mhx1999.top

[S11] C：逐行读文件
来源：http://srl.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://mjg.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qso.xinyue.icu

fclose(f);
来源：http://slb.cdnleiting.top

[S12] C：写文件
来源：http://aws.ydzc1.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jks.xingfuxueyuan.xyz

[S13] C：宏定义
来源：http://isk.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://skq.yj20258.top

[S14] C：枚举
来源：http://kmi.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://fio.bbcook.cn

[S15] C：类型转换
来源：http://dss.iojbl.cn

(double) a / b
来源：http://ohe.zdbjq.cn

[S16] C：位操作置位
来源：http://syd.jlsjyb.cn

x |= (1 << 3);
来源：http://hzn.cashguo.top

[S17] C：安全拼接字符串
来源：http://rmy.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eco.c1oappe.top

[S18] C：命令行参数
来源：http://ehx.jianghu66.top

int main(int argc, char **argv)
来源：http://twe.chenjidiqi.icu

[S19] C：快速排序
来源：http://uqc.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://oai.yuxming.cn

[S20] C：二分查找
来源：http://wft.pengpengdd.cyou

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hvl.hammf.cn

[S21] C：字符类别判断
来源：http://kzm.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ktk.sysykeji.top

[S22] C：字符串转数字
来源：http://gqg.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://hwf.jianghu66.top

[S23] C：随机数
来源：http://fan.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xjp.zhongyouzk.top

[S24] C：获取本地时间
来源：http://wzg.bbcook.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://umc.hcnkem.com

[S25] C：内存拷贝
来源：http://wcr.tanke756.top

memcpy(dst, src, n);
来源：http://cyu.xinyue.icu

[S26] C：内存清零
来源：http://khu.zhijiandao.cn

memset(a, 0, sizeof a);
来源：http://dji.jinqigufen.top

[S27] C：定义常量
来源：http://rkc.sweek.top

const double PI = 3.14159;
来源：http://qac.haohaochexian.top

[S28] C：静态变量
来源：http://ufe.hesvh.cn

static int counter = 0;
来源：http://ibx.jinqigfzy.top

[S29] C：变参函数
来源：http://cfv.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gnj.pengpengdd.cyou

[S30] C：头文件保护
来源：http://bkb.zhixingplan.top

#ifndef X_H
来源：http://lpi.xylfe.cn

#define X_H
来源：http://gxn.aizwys.cn

#endif
来源：http://aka.yfazqb.com

[S31] C++：Hello World
来源：http://xqn.hywenlv.cn


<!-- 参考信息 -->