代发 wailian999

[Q44] IN 子查询
来源：http://vnp.iojbl.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xtj.cashguo.top

[Q45] EXISTS 判断存在
来源：http://kyf.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nax.yuanzhike.top

[Q46] NOT EXISTS 判断不存在
来源：http://vvg.yangfankeji.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bmv.yuanzhike.top

[Q47] 与平均值比较
来源：http://yip.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pgw.sweek.top

[Q48] CTE 公用表表达式
来源：http://sgz.yangfankeji.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://koq.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://rwm.pengpengdd.cyou

[Q49] 更新单行
来源：http://vzd.sxryk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pzq.zycfv.cn

[Q50] 批量更新
来源：http://vhe.iojbl.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zwb.hesvh.cn

[Q51] 用子查询更新
来源：http://wqv.52xcode.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hmz.gzhubu.top

[Q52] 删除指定行
来源：http://jpx.fehbvm.com

DELETE FROM users WHERE id = 10;
来源：http://ops.ivvv.top

[Q53] 按条件删除
来源：http://edi.dashuyun.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lhp.cheryme.top

[Q54] 清空表
来源：http://dyd.birdmap.top

TRUNCATE TABLE logs;
来源：http://bdj.aibaodan.cn

[Q55] 排名（并列占位）
来源：http://sbh.havefunace.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://juc.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://ygl.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tfc.zhengqikj.top

[Q57] 行号
来源：http://khb.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xwo.dianchejie.cn

[Q58] 累计求和
来源：http://arv.zhaomingkeji.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bgh.zdqjudy.top

[Q59] 分组内累计
来源：http://cxj.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ond.gotoacloud.top

[Q60] 取上一行 / 下一行
来源：http://vow.zhengqikj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xtv.dianchejie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dfi.cheryme.top

[Q61] 移动平均
来源：http://mmt.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ndx.hesvh.cn

[Q62] 分组占比
来源：http://kpm.zhengqikj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rvq.jinghuilouyu.cn

[Q63] 开启事务
来源：http://xrz.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rvn.yvedp.cn

[Q64] 提交事务
来源：http://ezp.xuetiantiany.cn

COMMIT;
来源：http://txs.cheryme.top

[Q65] 回滚事务
来源：http://dra.quarkkingdee.top

ROLLBACK;
来源：http://jzk.chenzaomai.com

[Q66] 行锁查询
来源：http://dih.yj202588.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sdh.cashguo.top

[Q67] 设置隔离级别
来源：http://gqx.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jgp.xuanzx.com

[Q68] 保存点
来源：http://pli.zdqjudy.top

SAVEPOINT sp1;
来源：http://jyd.gotoacloud.top

ROLLBACK TO sp1;
来源：http://clh.meibo888.top

[Q69] 查看执行计划
来源：http://dec.yuxming.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iau.uphjek.com

[Q70] 更新统计信息
来源：http://tre.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://btg.jyoumei.cn

[Q71] 查看建表语句
来源：http://nti.hfpthk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gdq.tanke756.top

[Q72] 查看索引
来源：http://raj.gotoacloud.top

SHOW INDEX FROM users;
来源：http://gva.yanxiufei.cn

[Q73] 查看表状态
来源：http://yzr.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dbc.jinqigufen.top

[Q74] 强制使用索引
来源：http://wkc.kuanghao11.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ffr.ywan-chungtsiang.top

[Q75] 日期格式化
来源：http://chi.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yta.hysaishi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://itp.yj202588.top

[Q76] 按天统计
来源：http://ipm.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bsx.yuxming.cn

[Q77] 时间加减
来源：http://vgr.gogol.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zjx.mhx1999.top

[Q78] 当前时间
来源：http://sgk.wangdashe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qug.nanxuanxn.top

[Q79] 字符串拼接
来源：http://xjz.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bwf.sufxvd.cn

[Q80] 字符串截取
来源：http://kgp.iojbl.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rgt.hnxiangtu.top

[Q81] 字符串替换
来源：http://npn.52xcode.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yfw.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://ypn.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lnv.c1oappe.top

[Q83] 大小写转换
来源：http://nhl.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ndq.hysaishi.cn

[Q84] 去除首尾空格
来源：http://kba.zdbjq.cn

SELECT TRIM(name) FROM users;
来源：http://njf.zhengqikj.top

[Q85] 数值取整
来源：http://lcw.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://loe.shanyushiyangtech.top

[Q86] 读取 JSON 字段
来源：http://pmr.zhijiandao.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pmi.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://gwq.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lzy.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://jjd.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mjr.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yvp.ybcxt.top

[Q89] 判断表是否存在
来源：http://wlt.vehdjk.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nka.aibaodan.cn

[Q90] 生成序号列
来源：http://ywq.tarul.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jpy.9152youxi.cn

================================================================================
来源：http://ahi.nanxuanxn.top

R. Bash 专题
来源：http://wlq.shangyingyoupin.top

================================================================================
来源：http://qav.tianlin.xyz

[R01] shebang 与严格模式
来源：http://qas.ydjk.org.cn

#!/usr/bin/env bash
来源：http://fzx.nanxinkj.top

set -euo pipefail
来源：http://xzp.hywenlv.cn

[R02] 变量赋值与使用
来源：http://tlp.fehbvm.com

name="Tom"; echo "$name"
来源：http://etj.hnqzz.top

[R03] 只读变量
来源：http://cll.0kj1m.cn

readonly PI=3.14
来源：http://hqt.jinyuanbaomall.cn

[R04] 位置参数
来源：http://ygy.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hef.zdbjq.cn

[R05] 参数默认值
来源：http://lvt.ywan-chungtsiang.top

name="${1:-default}"
来源：http://hyi.nwbrower.top

[R06] 判断命令是否存在
来源：http://map.vqdsnc.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ycf.bjfxy.top

[R07] if 判断文件
来源：http://kyg.meibo888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fpb.yvedp.cn

[R08] 数值比较
来源：http://mpg.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mfq.ydzc1.top

[R09] 字符串比较
来源：http://jhg.fktsv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vht.52xcode.cn

[R10] 正则匹配
来源：http://ijo.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wxp.aizwys.cn

[R11] case 多分支
来源：http://nre.bjfxy.top

case "$1" in
来源：http://uhx.iojbl.cn

start) echo "启动" ;;
来源：http://tkg.yuanzhike.top

stop)  echo "停止" ;;
来源：http://oal.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://oyx.gzhubu.top

esac
来源：http://bdx.redwolf501.top

[R12] for 遍历文件
来源：http://csv.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://dqa.dashuyun.cn

[R13] for 计数循环
来源：http://fgs.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://nyh.xuetiantiany.cn

[R14] C 风格 for
来源：http://qth.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qua.zdbjq.cn

[R15] while 逐行读文件
来源：http://pxr.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pke.xylfe.cn

[R16] until 等待条件
来源：http://tyn.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wgr.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://eey.feifeiyinyue.top

arr=(a b c); echo "${arr[0]}"
来源：http://lgt.yuanzhike.top

[R18] 遍历数组
来源：http://nnz.vehdjk.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wsl.hfpthk.cn

[R19] 数组长度
来源：http://ssf.ydjk.org.cn

echo "${#arr[@]}"
来源：http://vky.dashuyun.cn

[R20] 关联数组（字典）
来源：http://wqd.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://csv.0kj1m.cn

[R21] 字符串长度
来源：http://lbs.zhixingplan.top

echo "${#s}"
来源：http://dgt.nwbrower.top

[R22] 截取子串
来源：http://ula.sysykeji.top

echo "${s:0:5}"
来源：http://dtd.tanke756.top

[R23] 字符串替换
来源：http://qvu.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zht.zhiwuduotai.top

[R24] 大小写转换
来源：http://qqg.nanxinkj.top

echo "${s^^}"; echo "${s,,}"
来源：http://zbq.zycfv.cn

[R25] 去后缀 / 去前缀
来源：http://fcn.zhijiandao.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://esa.guannengcc.top

[R26] 命令替换
来源：http://ice.yonumen.top

now=$(date +%F); echo "$now"
来源：http://ump.svipenyu.cn

[R27] 算术展开
来源：http://ujb.shuidangran.top

echo $((1 + 2 * 3))
来源：http://lmr.sxryk.cn

[R28] 浮点运算
来源：http://pas.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://sex.daria6918.cn

[R29] 定义函数
来源：http://ugh.yueranfly.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nry.haohaochexian.top

[R30] 函数返回状态码
来源：http://itt.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://qhy.hnqzz.top

[R31] 局部变量
来源：http://iwu.xinyue.icu

f() { local x=1; echo "$x"; }
来源：http://sob.tanke756.top

[R32] 参数个数校验
来源：http://ilm.hysaishi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fqt.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://ijv.fehbvm.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tlk.hongshengwenyu.top

[R34] 退出时清理
来源：http://srs.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eby.svipenyu.cn

[R35] 后台执行并等待
来源：http://afs.chenjidiqi.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://ffc.zdqjudy.top

[R36] 并发执行多个任务
来源：http://yte.meibo888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hqo.aibaodan.cn

[R37] 把输出赋给变量
来源：http://bca.316326.xyz

files=$(ls -1)
来源：http://uwz.feifeiyinyue.top

[R38] 管道串联
来源：http://kzp.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://nsn.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://gyb.havefunace.top

cmd > out.log 2>&1
来源：http://lhc.cqqwz.cn

[R40] 追加写日志
来源：http://umi.birdmap.top

echo "log" >> out.log
来源：http://ryi.hysaishi.cn

[R41] 丢弃输出
来源：http://jna.fengsongda.top

cmd >/dev/null 2>&1
来源：http://mhk.havefunace.top

[R42] 输入重定向
来源：http://cqz.hnqzz.top

wc -l < a.txt
来源：http://myq.fktsv.cn

[R43] 按名字查找文件
来源：http://gpx.tanke756.top

find . -name "*.log" -type f
来源：http://bgu.svipenyu.cn

[R44] 按修改时间查找
来源：http://elw.gotoacloud.top

find . -mtime -7 -type f
来源：http://ibt.jinyuanbaomall.cn

[R45] 批量删除
来源：http://ljg.hysaishi.cn

find . -name "*.tmp" -delete
来源：http://flw.hywenlv.cn

[R46] 递归替换文件内容
来源：http://njg.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bou.redwolf501.top

[R47] sed 单行替换
来源：http://zoc.chenzaomai.com

sed -i 's/foo/bar/g' a.txt
来源：http://lwq.yueranfly.top

[R48] awk 取指定列
来源：http://eyn.zdbjq.cn

awk '{print $1, $3}' a.txt
来源：http://pya.redwolf501.top

[R49] awk 带条件
来源：http://wga.iojbl.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jvf.mhx1999.top

[R50] awk 求和
来源：http://fdv.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nkw.tianlin.xyz

[R51] 排序去重取前几
来源：http://ndb.cheryme.top

sort a.txt | uniq -c | sort -rn | head
来源：http://eez.chenlongwang.top

[R52] 统计行数
来源：http://ndx.ydzc1.top

wc -l a.txt
来源：http://gfd.ppjwa.cn

[R53] 查看文件头与实时尾
来源：http://bwm.zdqjudy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yqm.ehwqpu.com

[R54] 比较两个文件
来源：http://dge.nwbrower.top

diff a.txt b.txt
来源：http://ova.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://mhq.snrcjt.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qbh.jyoumei.cn

[R56] 远程拷贝
来源：http://ylq.dianchejie.cn

scp file user@host:/path/
来源：http://unt.hfpthk.cn

[R57] 远程执行命令
来源：http://vad.bbcook.cn

ssh user@host 'uptime'
来源：http://xyw.epnwcf.com

[R58] 下载文件
来源：http://nnk.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lcq.xuetiantiany.cn

[R59] 发 POST JSON
来源：http://agg.jqgfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uav.zhixingplan.top

[R60] 只看 HTTP 状态码
来源：http://kbn.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uet.uphjek.com

[R61] 磁盘占用
来源：http://nmx.zhaomingkeji.xyz

df -h;  du -sh *
来源：http://cul.zhongyouzk.top

[R62] 找最占空间的文件
来源：http://ydf.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://zsb.ivvv.top

[R63] 内存与进程
来源：http://bdh.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://vxd.nanxuanxn.top

[R64] 结束进程
来源：http://fzf.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://jit.tanke756.top

[R65] 查看端口占用
来源：http://mna.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rvg.jiagoushi.top

[R66] 定时任务
来源：http://sfc.quarkkingdee.top

crontab -e;  crontab -l
来源：http://kyf.cheryme.top

[R67] 生成随机十六进制串
来源：http://bqf.havefunace.top

openssl rand -hex 16
来源：http://gsz.nanxinkj.top

[R68] 计算文件校验值
来源：http://bgq.yj20258888.top

sha256sum a.txt;  md5sum a.txt
来源：http://sig.wangshuangyany.cn

[R69] 生成随机密码
来源：http://dgo.ctjpmb.com

head -c 16 /dev/urandom | base64
来源：http://jhz.shuidangran.top

[R70] 时间戳与互转
来源：http://kqk.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://rrx.zycfv.cn

[R71] 日期格式化
来源：http://wzf.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kwi.gogol.net.cn

[R72] 等待端口就绪
来源：http://dyl.zhaomingkeji.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://van.cheryme.top

[R73] 分割大日志
来源：http://kdw.jlsjyb.cn

split -l 1000 big.log part_
来源：http://mdd.cashguo.top

[R74] 批量重命名
来源：http://zti.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ivp.ivvv.top

[R75] 导出环境变量
来源：http://drc.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://mot.yuanzhike.top

[R76] 使用临时文件
来源：http://jvt.zhengqikj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tad.gaohongyu789.top

[R77] 读取用户输入
来源：http://jip.ydjk.org.cn

read -rp "请输入: " ans
来源：http://cds.zhoulong.xyz

[R78] 交互式菜单
来源：http://cwg.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://eam.yfazqb.com

[R79] 解析命令行选项
来源：http://lyc.yuanzhike.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eom.hammf.cn

[R80] 查看脚本执行耗时
来源：http://fde.yvedp.cn

time ./run.sh
来源：http://iwq.chenjidiqi.icu

================================================================================
来源：http://vqn.guannengcc.top

S. C / C++ 专题
来源：http://wvk.quarkkingdee.top

================================================================================
来源：http://vch.snrcjt.cn

[S01] C：Hello World
来源：http://qlr.pengpengdd.cyou

#include <stdio.h>
来源：http://rcv.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://cec.ivvv.top

[S02] C：变量与格式化输出
来源：http://ksl.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://fhf.jinqigufen.top

[S03] C：读入整数
来源：http://iqv.epnwcf.com

int x; scanf("%d", &x);
来源：http://zhh.xuetiantiany.cn

[S04] C：字符串复制
来源：http://xcd.wangshuangyany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gjn.jqgfzy.top

[S05] C：字符串长度
来源：http://xav.hywenlv.cn

strlen(s)
来源：http://yjg.andypj.xyz

[S06] C：字符串比较
来源：http://rmo.iojbl.cn

strcmp(a, b) == 0
来源：http://dzy.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://cqq.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aco.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://fcg.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wnl.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://ugl.jinghuilouyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gxx.yfazqb.com

[S10] C：指针与解引用
来源：http://phu.bbcook.cn

int *p = &a;  *p = 5;
来源：http://mrz.meibo888.top

[S11] C：逐行读文件
来源：http://gao.c1oappe.top

FILE *f = fopen("a.txt", "r");
来源：http://rrp.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cgi.hfpthk.cn

fclose(f);
来源：http://nto.xylfe.cn

[S12] C：写文件
来源：http://ylw.jlsjyb.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zxn.guannengcc.top

[S13] C：宏定义
来源：http://iyr.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://myp.jqgufenzy.top

[S14] C：枚举
来源：http://mev.fktsv.cn


<!-- 参考信息 -->