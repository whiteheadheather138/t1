代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xhn.zhaomingkeji.xyz

[Q52] 删除指定行
来源：http://vmq.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://hrb.tanke756.top

[Q53] 按条件删除
来源：http://fau.yuxming.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cit.wangdashe.top

[Q54] 清空表
来源：http://izn.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://fhc.yongpay.top

[Q55] 排名（并列占位）
来源：http://maw.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://krp.sxryk.cn

[Q56] 密集排名（并列不占位）
来源：http://gfb.xinyue.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qhk.jqgufenzy.top

[Q57] 行号
来源：http://lez.zhijiandao.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hzc.fehbvm.com

[Q58] 累计求和
来源：http://wor.pengpengdd.cyou

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ckx.nwbrower.top

[Q59] 分组内累计
来源：http://plo.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iwd.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://ene.xingfuxueyuan.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eop.uphjek.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uam.hnxiangtu.top

[Q61] 移动平均
来源：http://nqz.shuidangran.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dtk.hywenlv.cn

[Q62] 分组占比
来源：http://riy.jyoumei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zxk.hywenlv.cn

[Q63] 开启事务
来源：http://kny.iojbl.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mmi.cdnleiting.top

[Q64] 提交事务
来源：http://xmz.tianlin.xyz

COMMIT;
来源：http://lig.zycfv.cn

[Q65] 回滚事务
来源：http://vpu.fengsongda.top

ROLLBACK;
来源：http://otb.yuanzhike.top

[Q66] 行锁查询
来源：http://usr.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kgj.cashguo.top

[Q67] 设置隔离级别
来源：http://sdc.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bwh.ybcxt.top

[Q68] 保存点
来源：http://wqj.ctjpmb.com

SAVEPOINT sp1;
来源：http://pox.jiagoushi.top

ROLLBACK TO sp1;
来源：http://hku.yueranfly.top

[Q69] 查看执行计划
来源：http://ydo.hywenlv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nqp.jinqigfzy.top

[Q70] 更新统计信息
来源：http://oxy.sxryk.cn

ANALYZE TABLE users;
来源：http://etx.gaohongyu789.top

[Q71] 查看建表语句
来源：http://hov.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://plz.guowangkeji.top

[Q72] 查看索引
来源：http://hue.cucudq.cn

SHOW INDEX FROM users;
来源：http://jjx.dashuyun.cn

[Q73] 查看表状态
来源：http://prm.iojbl.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://chi.xuanzx.com

[Q74] 强制使用索引
来源：http://uhf.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://itp.yanxiufei.cn

[Q75] 日期格式化
来源：http://yla.shanyushiyangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://saz.shangyingyoupin.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qlc.shzxlz.cn

[Q76] 按天统计
来源：http://zoa.52xcode.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ote.xziqi.cn

[Q77] 时间加减
来源：http://clb.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hsd.guowangkeji.top

[Q78] 当前时间
来源：http://vdg.hammf.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rul.bbcook.cn

[Q79] 字符串拼接
来源：http://jjg.zdbjq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wpp.quarkkingdee.top

[Q80] 字符串截取
来源：http://eac.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bfo.sufxvd.cn

[Q81] 字符串替换
来源：http://ryt.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lvj.birdmap.top

[Q82] 字符长度与字节长度
来源：http://ozf.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mvl.ivvv.top

[Q83] 大小写转换
来源：http://vie.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zsk.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://mvr.yangfankeji.com

SELECT TRIM(name) FROM users;
来源：http://tzh.yuanzhike.top

[Q85] 数值取整
来源：http://pld.zhongyouzk.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wuz.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://cvs.hongshengwenyu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zvj.fzhhl.top

[Q87] JSON 字段做条件
来源：http://mul.kuanghao11.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ebe.haohaochexian.top

[Q88] 行转列（条件聚合）
来源：http://xbq.pycfn.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gqu.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gmm.c1oappe.top

[Q89] 判断表是否存在
来源：http://dvl.gaohongyu789.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nhe.tian-w.cn

[Q90] 生成序号列
来源：http://fwl.svipenyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rze.tarul.cn

================================================================================
来源：http://kzb.yj20258888.top

R. Bash 专题
来源：http://fov.zycfv.cn

================================================================================
来源：http://atr.zdqjudy.top

[R01] shebang 与严格模式
来源：http://swl.chenzaomai.com

#!/usr/bin/env bash
来源：http://lqo.cashguo.top

set -euo pipefail
来源：http://vof.ppjwa.cn

[R02] 变量赋值与使用
来源：http://awi.sweek.top

name="Tom"; echo "$name"
来源：http://mup.snrcjt.cn

[R03] 只读变量
来源：http://lhr.yanxiufei.cn

readonly PI=3.14
来源：http://khe.svipenyu.cn

[R04] 位置参数
来源：http://ndy.aibaodan.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xam.vqdsnc.cn

[R05] 参数默认值
来源：http://ogu.hfpthk.cn

name="${1:-default}"
来源：http://zzr.sufxvd.cn

[R06] 判断命令是否存在
来源：http://ewl.zhaomingkeji.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lja.svipenyu.cn

[R07] if 判断文件
来源：http://joh.zhoulong.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kzr.tanke756.top

[R08] 数值比较
来源：http://awm.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gso.jlsjyb.cn

[R09] 字符串比较
来源：http://tou.zhongyouzk.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xfp.gzhubu.top

[R10] 正则匹配
来源：http://kam.shuidangran.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qdw.uphjek.com

[R11] case 多分支
来源：http://gud.hcnkem.com

case "$1" in
来源：http://nrk.ehwqpu.com

start) echo "启动" ;;
来源：http://vmj.sysykeji.top

stop)  echo "停止" ;;
来源：http://nlx.cheryme.top

*)     echo "未知命令" ;;
来源：http://wah.wangdashe.top

esac
来源：http://xcw.daxiang520.top

[R12] for 遍历文件
来源：http://fgw.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://roe.gzhubu.top

[R13] for 计数循环
来源：http://vay.yueranfly.top

for i in {1..10}; do echo "$i"; done
来源：http://zej.aibaodan.cn

[R14] C 风格 for
来源：http://ocw.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ifj.jqgufenzy.top

[R15] while 逐行读文件
来源：http://wdf.andypj.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zuz.hfpthk.cn

[R16] until 等待条件
来源：http://ynt.gotoacloud.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rpq.jlsjyb.cn

[R17] 数组定义与取值
来源：http://udv.guowangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://dix.jinqigufen.top

[R18] 遍历数组
来源：http://rnv.iojbl.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uqv.yangfankeji.com

[R19] 数组长度
来源：http://ffu.tanke756.top

echo "${#arr[@]}"
来源：http://ieq.9152youxi.cn

[R20] 关联数组（字典）
来源：http://dgg.vqdsnc.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ddb.smart0.xyz

[R21] 字符串长度
来源：http://tjl.jiagoushi.top

echo "${#s}"
来源：http://bcb.zycfv.cn

[R22] 截取子串
来源：http://pmb.jlsjyb.cn

echo "${s:0:5}"
来源：http://vww.jiagoushi.top

[R23] 字符串替换
来源：http://bey.jinghuilouyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rpy.xziqi.cn

[R24] 大小写转换
来源：http://yqc.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://oic.chenjidiqi.icu

[R25] 去后缀 / 去前缀
来源：http://pwh.xylfe.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://abh.nwbrower.top

[R26] 命令替换
来源：http://vpd.daria6918.cn

now=$(date +%F); echo "$now"
来源：http://kqc.wangdashe.top

[R27] 算术展开
来源：http://xpr.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://tzy.shanyushiyangtech.top

[R28] 浮点运算
来源：http://xms.yanxiufei.cn

echo "scale=2; 10/3" | bc
来源：http://den.xingfuxueyuan.xyz

[R29] 定义函数
来源：http://csv.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kmw.meibo888.top

[R30] 函数返回状态码
来源：http://jzn.xuetiantiany.cn

f() { return 0; }; f || echo "失败了"
来源：http://vfu.kuanghao11.cn

[R31] 局部变量
来源：http://lti.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://yaz.jinqigfzy.top

[R32] 参数个数校验
来源：http://okm.sufxvd.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fny.xuanzx.com

[R33] 捕获错误并提示行号
来源：http://qfz.fengsongda.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sem.hammf.cn

[R34] 退出时清理
来源：http://vlf.sweek.top

trap 'rm -f "$tmp"' EXIT
来源：http://rvf.bbcook.cn

[R35] 后台执行并等待
来源：http://dso.fengsongda.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lue.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://mdx.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bsl.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://aht.chenzaomai.com

files=$(ls -1)
来源：http://bvp.jlsjyb.cn

[R38] 管道串联
来源：http://uwv.redwolf501.top

cat a.txt | grep -i error | wc -l
来源：http://xto.jinyuanbaomall.cn

[R39] 重定向标准输出与错误
来源：http://qtu.svipenyu.cn

cmd > out.log 2>&1
来源：http://ymg.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://afl.shuidangran.top

echo "log" >> out.log
来源：http://foo.gotoacloud.top

[R41] 丢弃输出
来源：http://tfr.hnqzz.top

cmd >/dev/null 2>&1
来源：http://lmd.hongshengwenyu.top

[R42] 输入重定向
来源：http://qss.andypj.xyz

wc -l < a.txt
来源：http://ctk.zhijiandao.cn

[R43] 按名字查找文件
来源：http://fov.uphjek.com

find . -name "*.log" -type f
来源：http://oxf.yangfankeji.com

[R44] 按修改时间查找
来源：http://cfs.birdmap.top

find . -mtime -7 -type f
来源：http://uyh.tian-w.cn

[R45] 批量删除
来源：http://qsp.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://ymd.pengpengdd.cyou

[R46] 递归替换文件内容
来源：http://ugv.daria6918.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://avf.epnwcf.com

[R47] sed 单行替换
来源：http://sjv.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://hvl.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://ddg.zhijiandao.cn

awk '{print $1, $3}' a.txt
来源：http://xwb.hywenlv.cn

[R49] awk 带条件
来源：http://faj.tianlin.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yhy.smart0.xyz

[R50] awk 求和
来源：http://uyz.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://zxp.jinqigfzy.top

[R51] 排序去重取前几
来源：http://gyy.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hpi.chenjidiqi.icu

[R52] 统计行数
来源：http://tbm.jinghuilouyu.cn

wc -l a.txt
来源：http://dku.zdbjq.cn

[R53] 查看文件头与实时尾
来源：http://yes.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lxi.zhoulong.xyz

[R54] 比较两个文件
来源：http://ulh.fzhhl.top

diff a.txt b.txt
来源：http://ham.cucudq.cn

[R55] 压缩与解压
来源：http://pos.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wnb.jqgufenzy.top

[R56] 远程拷贝
来源：http://xts.52xcode.cn

scp file user@host:/path/
来源：http://zdj.ctjpmb.com

[R57] 远程执行命令
来源：http://xwv.shuidangran.top

ssh user@host 'uptime'
来源：http://hzn.yangfankeji.com

[R58] 下载文件
来源：http://fgo.fehbvm.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qbw.yj20258888.top

[R59] 发 POST JSON
来源：http://foo.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jak.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://lhc.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pte.jianghu66.top

[R61] 磁盘占用
来源：http://ube.jqgufenzy.top

df -h;  du -sh *
来源：http://lcs.9152youxi.cn

[R62] 找最占空间的文件
来源：http://rlw.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://fwp.hysaishi.cn

[R63] 内存与进程
来源：http://xty.feifeiyinyue.top

free -h;  ps aux | grep nginx
来源：http://mes.bjfxy.top

[R64] 结束进程
来源：http://hvr.wangshuangyany.cn

kill -9 $(pgrep -f app.py)
来源：http://eox.wangshuangyany.cn

[R65] 查看端口占用
来源：http://nrg.hywenlv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hxj.yvedp.cn

[R66] 定时任务
来源：http://jtx.yj20258888.top

crontab -e;  crontab -l
来源：http://zkj.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://ybd.yvedp.cn

openssl rand -hex 16
来源：http://hib.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://sta.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://crp.hongshengwenyu.top

[R69] 生成随机密码
来源：http://kdt.shanyushiyangkeji.top

head -c 16 /dev/urandom | base64
来源：http://scz.ydjk.org.cn

[R70] 时间戳与互转
来源：http://ney.shanyushiyangtech.top

date +%s;  date -d @1700000000
来源：http://iud.jiagoushi.top

[R71] 日期格式化
来源：http://lni.hongshengwenyu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tyq.aibaodan.cn

[R72] 等待端口就绪
来源：http://npd.guowangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rcl.yvedp.cn

[R73] 分割大日志
来源：http://yfa.ehwqpu.com

split -l 1000 big.log part_
来源：http://ors.cashguo.top

[R74] 批量重命名
来源：http://ydz.ctjpmb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gwv.ctjpmb.com

[R75] 导出环境变量
来源：http://ihm.zhiwuduotai.top

export PATH="$HOME/bin:$PATH"
来源：http://lai.hywenlv.cn

[R76] 使用临时文件
来源：http://bmt.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ixc.redwolf501.top

[R77] 读取用户输入
来源：http://bxu.zhiwuduotai.top

read -rp "请输入: " ans
来源：http://sil.feifeiyinyue.top

[R78] 交互式菜单
来源：http://kni.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ncl.sweek.top

[R79] 解析命令行选项
来源：http://wuv.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://quh.xinyue.icu

[R80] 查看脚本执行耗时
来源：http://uhz.daria6918.cn

time ./run.sh
来源：http://gis.nwbrower.top

================================================================================
来源：http://iqm.uphjek.com

S. C / C++ 专题
来源：http://uxp.hfpthk.cn

================================================================================
来源：http://jps.hysaishi.cn

[S01] C：Hello World
来源：http://qnc.shanyushiyangkeji.top

#include <stdio.h>
来源：http://cfa.haohaochexian.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hcp.quarkkingdee.top

[S02] C：变量与格式化输出
来源：http://dxk.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://cga.xinyue.icu

[S03] C：读入整数
来源：http://qio.jianghu66.top

int x; scanf("%d", &x);
来源：http://bct.zhaomingkeji.xyz

[S04] C：字符串复制
来源：http://cjt.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://htj.9152youxi.cn

[S05] C：字符串长度
来源：http://waj.yueranfly.top

strlen(s)
来源：http://cot.shanyushiyangtech.top

[S06] C：字符串比较
来源：http://vlg.meibo888.top

strcmp(a, b) == 0
来源：http://ivg.ybcxt.top

[S07] C：数组遍历求和
来源：http://qdq.jinqigfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ods.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://tca.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mkd.zhongyouzk.top

[S09] C：结构体定义与初始化
来源：http://dfk.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kce.yfazqb.com

[S10] C：指针与解引用
来源：http://hid.nwbrower.top

int *p = &a;  *p = 5;
来源：http://swh.yanxiufei.cn

[S11] C：逐行读文件
来源：http://ysc.uphjek.com

FILE *f = fopen("a.txt", "r");
来源：http://lmt.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vwd.fehbvm.com

fclose(f);
来源：http://xkr.sweek.top

[S12] C：写文件
来源：http://wct.jyoumei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hxf.zhiwuduotai.top

[S13] C：宏定义
来源：http://emx.zhengqikj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://way.pycfn.com

[S14] C：枚举
来源：http://ozf.ybcxt.top

enum Color { RED, GREEN, BLUE };
来源：http://iuj.hywenlv.cn

[S15] C：类型转换
来源：http://bzu.aibaodan.cn

(double) a / b
来源：http://ssq.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://gsy.shanyushiyangtech.top

x |= (1 << 3);
来源：http://woj.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://bnl.gzhubu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cxq.pycfn.com

[S18] C：命令行参数
来源：http://epb.ydzc1.top

int main(int argc, char **argv)
来源：http://mud.ivvv.top

[S19] C：快速排序
来源：http://uxs.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://hom.jianghu66.top

[S20] C：二分查找
来源：http://jmv.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qma.hesvh.cn

[S21] C：字符类别判断
来源：http://vnj.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cjf.haohaochexian.top

[S22] C：字符串转数字
来源：http://jxg.mhx1999.top


<!-- 参考信息 -->