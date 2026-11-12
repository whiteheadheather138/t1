代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://asc.havefunace.top

[Q60] 取上一行 / 下一行
来源：http://wtb.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gnn.jiagoushi.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qmq.pengpengdd.cyou

[Q61] 移动平均
来源：http://pfs.cdnleiting.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xfv.zhongyouzk.top

[Q62] 分组占比
来源：http://swf.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://snu.sweek.top

[Q63] 开启事务
来源：http://tjd.ctjpmb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://nvt.hywenlv.cn

[Q64] 提交事务
来源：http://awu.yj20258.top

COMMIT;
来源：http://vmm.jyoumei.cn

[Q65] 回滚事务
来源：http://jnf.wangdashe.top

ROLLBACK;
来源：http://htd.sxryk.cn

[Q66] 行锁查询
来源：http://wtk.xinyue.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nnt.316326.xyz

[Q67] 设置隔离级别
来源：http://iuv.sysykeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lrf.tian-w.cn

[Q68] 保存点
来源：http://ojv.zhixingplan.top

SAVEPOINT sp1;
来源：http://xuy.cdnleiting.top

ROLLBACK TO sp1;
来源：http://pss.epnwcf.com

[Q69] 查看执行计划
来源：http://gku.nanxinkj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qyz.xylfe.cn

[Q70] 更新统计信息
来源：http://jir.nanxinkj.top

ANALYZE TABLE users;
来源：http://fzm.tianlin.xyz

[Q71] 查看建表语句
来源：http://llx.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zsi.zhoulong.xyz

[Q72] 查看索引
来源：http://qih.gaohongyu789.top

SHOW INDEX FROM users;
来源：http://elo.cdnleiting.top

[Q73] 查看表状态
来源：http://slq.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ndx.andypj.xyz

[Q74] 强制使用索引
来源：http://caw.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ijx.jiagoushi.top

[Q75] 日期格式化
来源：http://fyd.daria6918.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eyn.tianlin.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ldn.xinyue.icu

[Q76] 按天统计
来源：http://iqi.xuanzx.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pxt.nanxinkj.top

[Q77] 时间加减
来源：http://fux.quarkkingdee.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pbt.xuanzx.com

[Q78] 当前时间
来源：http://lpo.yj20258888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ovt.ybcxt.top

[Q79] 字符串拼接
来源：http://hvx.hammf.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uvn.uphjek.com

[Q80] 字符串截取
来源：http://ygh.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://upz.pengpengdd.cyou

[Q81] 字符串替换
来源：http://vyi.bjfxy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rmj.yvedp.cn

[Q82] 字符长度与字节长度
来源：http://egq.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://byz.gaohongyu789.top

[Q83] 大小写转换
来源：http://bty.hywenlv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dli.sufxvd.cn

[Q84] 去除首尾空格
来源：http://cjf.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://lvy.jqgfzy.top

[Q85] 数值取整
来源：http://wau.ydjk.org.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cpi.yfazqb.com

[Q86] 读取 JSON 字段
来源：http://urs.hysaishi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bgt.hnxiangtu.top

[Q87] JSON 字段做条件
来源：http://hrs.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bby.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://lsq.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fbe.hesvh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gso.9152youxi.cn

[Q89] 判断表是否存在
来源：http://tbl.cdnleiting.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tfv.yongpay.top

[Q90] 生成序号列
来源：http://yzv.epnwcf.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://esh.jinyuanbaomall.cn

================================================================================
来源：http://cve.vehdjk.com

R. Bash 专题
来源：http://jnl.jinqigufen.top

================================================================================
来源：http://djj.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://vpq.ehwqpu.com

#!/usr/bin/env bash
来源：http://hne.fehbvm.com

set -euo pipefail
来源：http://dyn.jyoumei.cn

[R02] 变量赋值与使用
来源：http://ssc.tianlin.xyz

name="Tom"; echo "$name"
来源：http://fcw.hongshengwenyu.top

[R03] 只读变量
来源：http://vnr.gogol.net.cn

readonly PI=3.14
来源：http://tln.9152youxi.cn

[R04] 位置参数
来源：http://bwh.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jhq.gzhubu.top

[R05] 参数默认值
来源：http://yts.cashguo.top

name="${1:-default}"
来源：http://xmf.ivvv.top

[R06] 判断命令是否存在
来源：http://myn.havefunace.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eqg.9152youxi.cn

[R07] if 判断文件
来源：http://mpe.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zbw.fengsongda.top

[R08] 数值比较
来源：http://jfs.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yer.fengsongda.top

[R09] 字符串比较
来源：http://tkr.jinqigufen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rrv.xuanzx.com

[R10] 正则匹配
来源：http://vod.nwbrower.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fky.cqqwz.cn

[R11] case 多分支
来源：http://qhj.shuidangran.top

case "$1" in
来源：http://nar.jinyuanbaomall.cn

start) echo "启动" ;;
来源：http://xpr.hfpthk.cn

stop)  echo "停止" ;;
来源：http://hrm.tian-w.cn

*)     echo "未知命令" ;;
来源：http://jbj.hcnkem.com

esac
来源：http://tkc.fktsv.cn

[R12] for 遍历文件
来源：http://qqm.jinqigfzy.top

for f in *.txt; do echo "$f"; done
来源：http://sfs.yj20258888.top

[R13] for 计数循环
来源：http://wtg.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://ndj.zhoulong.xyz

[R14] C 风格 for
来源：http://vru.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vnt.daxiang520.top

[R15] while 逐行读文件
来源：http://mnh.fzhhl.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ovg.52xcode.cn

[R16] until 等待条件
来源：http://syo.epnwcf.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bev.hcnkem.com

[R17] 数组定义与取值
来源：http://pcv.wangshuangyany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zhl.cucudq.cn

[R18] 遍历数组
来源：http://xru.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fmr.chenlongwang.top

[R19] 数组长度
来源：http://xmo.jlsjyb.cn

echo "${#arr[@]}"
来源：http://baf.birdmap.top

[R20] 关联数组（字典）
来源：http://kfh.wangdashe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jkw.tanke756.top

[R21] 字符串长度
来源：http://bak.ydzc1.top

echo "${#s}"
来源：http://zvy.zhongyouzk.top

[R22] 截取子串
来源：http://txg.xylfe.cn

echo "${s:0:5}"
来源：http://hew.cheryme.top

[R23] 字符串替换
来源：http://our.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kxs.xingfuxueyuan.xyz

[R24] 大小写转换
来源：http://jol.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://vyj.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://exq.cheryme.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ntq.yongpay.top

[R26] 命令替换
来源：http://xwt.zycfv.cn

now=$(date +%F); echo "$now"
来源：http://etu.cheryme.top

[R27] 算术展开
来源：http://guw.daria6918.cn

echo $((1 + 2 * 3))
来源：http://wan.cucudq.cn

[R28] 浮点运算
来源：http://eqj.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://oks.svipenyu.cn

[R29] 定义函数
来源：http://vci.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pjm.jyoumei.cn

[R30] 函数返回状态码
来源：http://ofo.xziqi.cn

f() { return 0; }; f || echo "失败了"
来源：http://cgw.sweek.top

[R31] 局部变量
来源：http://rgi.xuanzx.com

f() { local x=1; echo "$x"; }
来源：http://mdp.ppjwa.cn

[R32] 参数个数校验
来源：http://xkj.chenlongwang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sme.mhx1999.top

[R33] 捕获错误并提示行号
来源：http://geu.guannengcc.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kls.sxryk.cn

[R34] 退出时清理
来源：http://ipp.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://dnd.pycfn.com

[R35] 后台执行并等待
来源：http://mpm.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://poa.xuanzx.com

[R36] 并发执行多个任务
来源：http://yed.ydjk.org.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yzm.9152youxi.cn

[R37] 把输出赋给变量
来源：http://jll.tianlin.xyz

files=$(ls -1)
来源：http://wks.kuanghao11.cn

[R38] 管道串联
来源：http://pep.jyoumei.cn

cat a.txt | grep -i error | wc -l
来源：http://qiy.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://kff.birdmap.top

cmd > out.log 2>&1
来源：http://ufw.daxiang520.top

[R40] 追加写日志
来源：http://mrf.zhaomingkeji.xyz

echo "log" >> out.log
来源：http://saf.havefunace.top

[R41] 丢弃输出
来源：http://qpq.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://oth.hesvh.cn

[R42] 输入重定向
来源：http://srh.iojbl.cn

wc -l < a.txt
来源：http://mfh.nanxuanxn.top

[R43] 按名字查找文件
来源：http://dri.havefunace.top

find . -name "*.log" -type f
来源：http://pvn.jlsjyb.cn

[R44] 按修改时间查找
来源：http://puu.shuidangran.top

find . -mtime -7 -type f
来源：http://iwq.xylfe.cn

[R45] 批量删除
来源：http://uwy.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://ihr.smart0.xyz

[R46] 递归替换文件内容
来源：http://eqs.zhijiandao.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yix.svipenyu.cn

[R47] sed 单行替换
来源：http://umn.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mag.guowangkeji.top

[R48] awk 取指定列
来源：http://azq.aizwys.cn

awk '{print $1, $3}' a.txt
来源：http://ply.tarul.cn

[R49] awk 带条件
来源：http://hzt.hnqzz.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ezq.sufxvd.cn

[R50] awk 求和
来源：http://mtw.jqgfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://zgj.dashuyun.cn

[R51] 排序去重取前几
来源：http://vgj.cheryme.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fwr.sysykeji.top

[R52] 统计行数
来源：http://wuw.tian-w.cn

wc -l a.txt
来源：http://kvx.vehdjk.com

[R53] 查看文件头与实时尾
来源：http://erh.yangfankeji.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bka.daria6918.cn

[R54] 比较两个文件
来源：http://gno.jqgufenzy.top

diff a.txt b.txt
来源：http://rid.hysaishi.cn

[R55] 压缩与解压
来源：http://txz.zhixingplan.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rrd.andypj.xyz

[R56] 远程拷贝
来源：http://xis.birdmap.top

scp file user@host:/path/
来源：http://ymw.c1oappe.top

[R57] 远程执行命令
来源：http://wdr.yj20258.top

ssh user@host 'uptime'
来源：http://oqb.jqgufenzy.top

[R58] 下载文件
来源：http://duq.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://stf.yonumen.top

[R59] 发 POST JSON
来源：http://eye.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ssz.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://oxy.ydzc1.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://spv.xylfe.cn

[R61] 磁盘占用
来源：http://tdd.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://ank.vqdsnc.cn

[R62] 找最占空间的文件
来源：http://kia.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://xzf.chenjidiqi.icu

[R63] 内存与进程
来源：http://lpo.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://jyb.gogol.net.cn

[R64] 结束进程
来源：http://muo.yfazqb.com

kill -9 $(pgrep -f app.py)
来源：http://pkt.chenlongwang.top

[R65] 查看端口占用
来源：http://usp.cqqwz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uri.dianchejie.cn

[R66] 定时任务
来源：http://ony.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://sne.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://qsc.hesvh.cn

openssl rand -hex 16
来源：http://xik.yuxming.cn

[R68] 计算文件校验值
来源：http://eoi.cqqwz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://crw.ydzc1.top

[R69] 生成随机密码
来源：http://dql.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://fyz.yj20258888.top

[R70] 时间戳与互转
来源：http://vid.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://dpn.zycfv.cn

[R71] 日期格式化
来源：http://vhn.snrcjt.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cfw.yj202588.top

[R72] 等待端口就绪
来源：http://tyb.yfazqb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://yvw.tanke756.top

[R73] 分割大日志
来源：http://hcy.sysykeji.top

split -l 1000 big.log part_
来源：http://gov.tanke756.top

[R74] 批量重命名
来源：http://ohu.fktsv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://shj.ctjpmb.com

[R75] 导出环境变量
来源：http://cwy.smart0.xyz

export PATH="$HOME/bin:$PATH"
来源：http://eoz.yuanzhike.top

[R76] 使用临时文件
来源：http://sto.zhengqikj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ylo.shuidangran.top

[R77] 读取用户输入
来源：http://nzj.xziqi.cn

read -rp "请输入: " ans
来源：http://glf.yj202588.top

[R78] 交互式菜单
来源：http://unj.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jfr.redwolf501.top

[R79] 解析命令行选项
来源：http://vmo.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jfb.zdbjq.cn

[R80] 查看脚本执行耗时
来源：http://hwu.hfpthk.cn

time ./run.sh
来源：http://avb.yangfankeji.com

================================================================================
来源：http://ute.shanyushiyangkeji.top

S. C / C++ 专题
来源：http://jgv.zhiwuduotai.top

================================================================================
来源：http://jdx.yanxiufei.cn

[S01] C：Hello World
来源：http://yts.guowangkeji.top

#include <stdio.h>
来源：http://hdp.cheryme.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rze.fzhhl.top

[S02] C：变量与格式化输出
来源：http://jzy.guannengcc.top

int a = 10; printf("%d\n", a);
来源：http://eur.aibaodan.cn

[S03] C：读入整数
来源：http://xhb.bbcook.cn

int x; scanf("%d", &x);
来源：http://cxg.daxiang520.top

[S04] C：字符串复制
来源：http://uhu.haohaochexian.top

char dst[32]; strcpy(dst, "hi");
来源：http://qtk.nanxinkj.top

[S05] C：字符串长度
来源：http://jfx.jqgfzy.top

strlen(s)
来源：http://ivt.xingfuxueyuan.xyz

[S06] C：字符串比较
来源：http://jeg.hysaishi.cn

strcmp(a, b) == 0
来源：http://ljb.andypj.xyz

[S07] C：数组遍历求和
来源：http://qqt.dianchejie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sti.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://qmd.daria6918.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rcc.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://hpq.haohaochexian.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nbf.hysaishi.cn

[S10] C：指针与解引用
来源：http://vvx.c1oappe.top

int *p = &a;  *p = 5;
来源：http://ayb.zdbjq.cn

[S11] C：逐行读文件
来源：http://nlp.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://pgo.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yzn.hfpthk.cn

fclose(f);
来源：http://qir.havefunace.top

[S12] C：写文件
来源：http://scj.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ppe.smart0.xyz

[S13] C：宏定义
来源：http://gze.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sqt.yvedp.cn

[S14] C：枚举
来源：http://wce.316326.xyz

enum Color { RED, GREEN, BLUE };
来源：http://ibp.gogol.net.cn

[S15] C：类型转换
来源：http://ais.shanyushiyangtech.top

(double) a / b
来源：http://exo.meibo888.top

[S16] C：位操作置位
来源：http://xko.shuidangran.top

x |= (1 << 3);
来源：http://eat.uphjek.com

[S17] C：安全拼接字符串
来源：http://yrl.kuanghao11.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wjv.zdbjq.cn

[S18] C：命令行参数
来源：http://zqs.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://mei.hcnkem.com

[S19] C：快速排序
来源：http://vfr.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://nrc.andypj.xyz

[S20] C：二分查找
来源：http://ccp.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ivt.sweek.top

[S21] C：字符类别判断
来源：http://sej.guowangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tkd.ehwqpu.com

[S22] C：字符串转数字
来源：http://vjg.fengsongda.top

atoi("42");  strtod("3.14", NULL);
来源：http://all.sufxvd.cn

[S23] C：随机数
来源：http://uak.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vlr.fengsongda.top

[S24] C：获取本地时间
来源：http://eeb.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ykl.xziqi.cn

[S25] C：内存拷贝
来源：http://qux.jianghu66.top

memcpy(dst, src, n);
来源：http://dwe.smart0.xyz

[S26] C：内存清零
来源：http://rpa.sxryk.cn

memset(a, 0, sizeof a);
来源：http://jsa.shzxlz.cn

[S27] C：定义常量
来源：http://vax.zhijiandao.cn

const double PI = 3.14159;
来源：http://uur.tianlin.xyz

[S28] C：静态变量
来源：http://drx.zhoulong.xyz

static int counter = 0;
来源：http://aas.guowangkeji.top

[S29] C：变参函数
来源：http://wuv.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vnd.xinyue.icu

[S30] C：头文件保护
来源：http://hnb.jinyuanbaomall.cn


<!-- 参考信息 -->