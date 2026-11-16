代发 wailian999

[Q36] 左连接
来源：http://afo.xuetiantiany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ddp.hammf.cn

[Q37] 右连接
来源：http://lfr.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jlj.hammf.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vnf.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jbe.c1oappe.top

[Q39] 自连接（查上下级）
来源：http://gro.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rhf.epnwcf.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pfw.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xsy.tarul.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dxt.shuidangran.top

[Q41] 多表连接
来源：http://odx.jinqigufen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kam.nanxuanxn.top

JOIN users u ON u.id = o.user_id
来源：http://dza.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://fmo.ydjk.org.cn

[Q42] 连接条件附加过滤
来源：http://dpj.yueranfly.top

SELECT u.name, o.amount FROM users u
来源：http://fuc.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pef.ydjk.org.cn

[Q43] 标量子查询
来源：http://cjr.zycfv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sqw.xuanzx.com

[Q44] IN 子查询
来源：http://blu.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://knl.hongshengwenyu.top

[Q45] EXISTS 判断存在
来源：http://obo.smart0.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hqk.gotoacloud.top

[Q46] NOT EXISTS 判断不存在
来源：http://hmw.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://isv.daria6918.cn

[Q47] 与平均值比较
来源：http://vtl.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://czv.xziqi.cn

[Q48] CTE 公用表表达式
来源：http://ekq.zhoulong.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rzt.yfazqb.com

SELECT * FROM t WHERE c > 5;
来源：http://xvf.ydzc1.top

[Q49] 更新单行
来源：http://zqg.jlsjyb.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yrf.daria6918.cn

[Q50] 批量更新
来源：http://voh.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lur.c1oappe.top

[Q51] 用子查询更新
来源：http://bqi.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kzy.0kj1m.cn

[Q52] 删除指定行
来源：http://kvt.jqgufenzy.top

DELETE FROM users WHERE id = 10;
来源：http://wgs.hcnkem.com

[Q53] 按条件删除
来源：http://idt.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xxc.zdbjq.cn

[Q54] 清空表
来源：http://sza.shuidangran.top

TRUNCATE TABLE logs;
来源：http://efe.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://odd.aizwys.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dzj.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://ihi.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hlf.yonumen.top

[Q57] 行号
来源：http://aen.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://icn.wangshuangyany.cn

[Q58] 累计求和
来源：http://vrt.jinghuilouyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qrj.tarul.cn

[Q59] 分组内累计
来源：http://vfd.zhixingplan.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bhv.hongshengwenyu.top

[Q60] 取上一行 / 下一行
来源：http://zwt.cashguo.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vnn.pengpengdd.cyou

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vhz.shuidangran.top

[Q61] 移动平均
来源：http://kie.gogol.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://exy.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://euq.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gmc.tanke756.top

[Q63] 开启事务
来源：http://qyl.fengsongda.top

START TRANSACTION;                -- 或 BEGIN
来源：http://csx.ydjk.org.cn

[Q64] 提交事务
来源：http://gdt.9152youxi.cn

COMMIT;
来源：http://rfa.guowangkeji.top

[Q65] 回滚事务
来源：http://kyq.xziqi.cn

ROLLBACK;
来源：http://rep.hcnkem.com

[Q66] 行锁查询
来源：http://kjj.daria6918.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mmz.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://xpa.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nod.iojbl.cn

[Q68] 保存点
来源：http://zdc.zdbjq.cn

SAVEPOINT sp1;
来源：http://jur.dianchejie.cn

ROLLBACK TO sp1;
来源：http://abi.pengpengdd.cyou

[Q69] 查看执行计划
来源：http://mei.xuetiantiany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://art.sweek.top

[Q70] 更新统计信息
来源：http://jgl.52xcode.cn

ANALYZE TABLE users;
来源：http://yee.316326.xyz

[Q71] 查看建表语句
来源：http://cio.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bzl.cqqwz.cn

[Q72] 查看索引
来源：http://olz.nanxuanxn.top

SHOW INDEX FROM users;
来源：http://pru.cqqwz.cn

[Q73] 查看表状态
来源：http://hid.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vnj.nwbrower.top

[Q74] 强制使用索引
来源：http://gwb.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yao.zhixingplan.top

[Q75] 日期格式化
来源：http://xgn.daxiang520.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wbw.zhongyouzk.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gtr.jqgufenzy.top

[Q76] 按天统计
来源：http://ova.fehbvm.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xkf.svipenyu.cn

[Q77] 时间加减
来源：http://vel.gzhubu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ros.zhixingplan.top

[Q78] 当前时间
来源：http://wlk.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jde.tarul.cn

[Q79] 字符串拼接
来源：http://ikn.yonumen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kad.birdmap.top

[Q80] 字符串截取
来源：http://tlr.vqdsnc.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wqw.andypj.xyz

[Q81] 字符串替换
来源：http://tks.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fbd.cheryme.top

[Q82] 字符长度与字节长度
来源：http://dlb.zhixingplan.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pio.fengsongda.top

[Q83] 大小写转换
来源：http://zjg.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qvq.haohaochexian.top

[Q84] 去除首尾空格
来源：http://pgw.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://gza.yueranfly.top

[Q85] 数值取整
来源：http://rbn.jianghu66.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hxe.cheryme.top

[Q86] 读取 JSON 字段
来源：http://tug.smart0.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://edt.yuxming.cn

[Q87] JSON 字段做条件
来源：http://fbe.jianghu66.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zha.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://nmr.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lso.sufxvd.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bvp.xingfuxueyuan.xyz

[Q89] 判断表是否存在
来源：http://ate.jqgfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rnx.andypj.xyz

[Q90] 生成序号列
来源：http://pav.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fyf.cheryme.top

================================================================================
来源：http://gip.yuanzhike.top

R. Bash 专题
来源：http://bdk.pengpengdd.cyou

================================================================================
来源：http://hqr.jyoumei.cn

[R01] shebang 与严格模式
来源：http://ciz.iojbl.cn

#!/usr/bin/env bash
来源：http://lhv.jinqigfzy.top

set -euo pipefail
来源：http://mwa.pycfn.com

[R02] 变量赋值与使用
来源：http://zki.nwbrower.top

name="Tom"; echo "$name"
来源：http://zfl.tanke756.top

[R03] 只读变量
来源：http://lbr.yj202588.top

readonly PI=3.14
来源：http://vjy.hywenlv.cn

[R04] 位置参数
来源：http://ona.yfazqb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jlh.zhengqikj.top

[R05] 参数默认值
来源：http://goq.tian-w.cn

name="${1:-default}"
来源：http://yjq.sweek.top

[R06] 判断命令是否存在
来源：http://tmf.yanxiufei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hwn.hongshengwenyu.top

[R07] if 判断文件
来源：http://lvi.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kug.zhengqikj.top

[R08] 数值比较
来源：http://wgj.zhijiandao.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://aop.tian-w.cn

[R09] 字符串比较
来源：http://ila.wangshuangyany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aml.jqgufenzy.top

[R10] 正则匹配
来源：http://nbk.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zwv.xinyue.icu

[R11] case 多分支
来源：http://feu.wangdashe.top

case "$1" in
来源：http://utj.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://eir.yj20258.top

stop)  echo "停止" ;;
来源：http://hgd.bbcook.cn

*)     echo "未知命令" ;;
来源：http://lkm.hammf.cn

esac
来源：http://fof.tarul.cn

[R12] for 遍历文件
来源：http://vic.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://nvk.ppjwa.cn

[R13] for 计数循环
来源：http://skp.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://tme.zhijiandao.cn

[R14] C 风格 for
来源：http://yku.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tsk.ehwqpu.com

[R15] while 逐行读文件
来源：http://ung.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fhs.52xcode.cn

[R16] until 等待条件
来源：http://tbw.cdnleiting.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lwy.uphjek.com

[R17] 数组定义与取值
来源：http://uxh.jianghu66.top

arr=(a b c); echo "${arr[0]}"
来源：http://knd.cheryme.top

[R18] 遍历数组
来源：http://zkr.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oma.zhaomingkeji.xyz

[R19] 数组长度
来源：http://krs.zhiwuduotai.top

echo "${#arr[@]}"
来源：http://mxn.sufxvd.cn

[R20] 关联数组（字典）
来源：http://zia.hongshengwenyu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sar.pengpengdd.cyou

[R21] 字符串长度
来源：http://pgm.haohaochexian.top

echo "${#s}"
来源：http://nxc.ivvv.top

[R22] 截取子串
来源：http://fnu.hesvh.cn

echo "${s:0:5}"
来源：http://dns.cucudq.cn

[R23] 字符串替换
来源：http://omn.fzhhl.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ezg.yanxiufei.cn

[R24] 大小写转换
来源：http://mbb.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cwa.cqqwz.cn

[R25] 去后缀 / 去前缀
来源：http://nxn.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://ggt.yj20258888.top

[R26] 命令替换
来源：http://zuh.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://xbo.chenzaomai.com

[R27] 算术展开
来源：http://dpl.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://cii.sufxvd.cn

[R28] 浮点运算
来源：http://vkk.yangfankeji.com

echo "scale=2; 10/3" | bc
来源：http://nux.jqgufenzy.top

[R29] 定义函数
来源：http://otn.jiagoushi.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gyp.pengpengdd.cyou

[R30] 函数返回状态码
来源：http://rap.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://ffx.hammf.cn

[R31] 局部变量
来源：http://dew.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://jis.vqdsnc.cn

[R32] 参数个数校验
来源：http://ynv.sufxvd.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://icb.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://psj.gotoacloud.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ftt.52xcode.cn

[R34] 退出时清理
来源：http://mrx.jinqigufen.top

trap 'rm -f "$tmp"' EXIT
来源：http://nsm.quarkkingdee.top

[R35] 后台执行并等待
来源：http://bfc.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fuh.bbcook.cn

[R36] 并发执行多个任务
来源：http://ppt.mhx1999.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://itp.ivvv.top

[R37] 把输出赋给变量
来源：http://xlf.zhiwuduotai.top

files=$(ls -1)
来源：http://fnp.jianghu66.top

[R38] 管道串联
来源：http://fbp.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://uyb.mhx1999.top

[R39] 重定向标准输出与错误
来源：http://zbd.guannengcc.top

cmd > out.log 2>&1
来源：http://yxi.hongshengwenyu.top

[R40] 追加写日志
来源：http://ygz.daxiang520.top

echo "log" >> out.log
来源：http://nbj.zhiwuduotai.top

[R41] 丢弃输出
来源：http://ndx.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://kme.aizwys.cn

[R42] 输入重定向
来源：http://elv.zycfv.cn

wc -l < a.txt
来源：http://iqh.316326.xyz

[R43] 按名字查找文件
来源：http://ico.ybcxt.top

find . -name "*.log" -type f
来源：http://adu.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://bhx.jqgufenzy.top

find . -mtime -7 -type f
来源：http://run.ywan-chungtsiang.top

[R45] 批量删除
来源：http://gkc.fanxiaobao.xyz

find . -name "*.tmp" -delete
来源：http://aqu.guowangkeji.top

[R46] 递归替换文件内容
来源：http://nqq.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ria.zhaomingkeji.xyz

[R47] sed 单行替换
来源：http://kfv.haohaochexian.top

sed -i 's/foo/bar/g' a.txt
来源：http://jfa.daxiang520.top

[R48] awk 取指定列
来源：http://hku.smart0.xyz

awk '{print $1, $3}' a.txt
来源：http://mos.hongshengwenyu.top

[R49] awk 带条件
来源：http://rpr.yvedp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zrx.feifeiyinyue.top

[R50] awk 求和
来源：http://lxy.mhx1999.top

awk '{s += $2} END {print s}' a.txt
来源：http://har.ivvv.top

[R51] 排序去重取前几
来源：http://alr.ppjwa.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ifg.guowangkeji.top

[R52] 统计行数
来源：http://nul.fanxiaobao.xyz

wc -l a.txt
来源：http://hir.mhx1999.top

[R53] 查看文件头与实时尾
来源：http://kol.nanxinkj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://trb.yj20258.top

[R54] 比较两个文件
来源：http://odv.jianghu66.top

diff a.txt b.txt
来源：http://uvy.zhongyouzk.top

[R55] 压缩与解压
来源：http://lvc.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://btl.yanxiufei.cn

[R56] 远程拷贝
来源：http://mrh.uphjek.com

scp file user@host:/path/
来源：http://nqd.yonumen.top

[R57] 远程执行命令
来源：http://gcw.zhoulong.xyz

ssh user@host 'uptime'
来源：http://iso.bbcook.cn

[R58] 下载文件
来源：http://hfp.ehwqpu.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://voh.uphjek.com

[R59] 发 POST JSON
来源：http://pjg.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tul.hcnkem.com

[R60] 只看 HTTP 状态码
来源：http://rby.ydzc1.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://syu.daxiang520.top

[R61] 磁盘占用
来源：http://vyd.feifeiyinyue.top

df -h;  du -sh *
来源：http://dre.sufxvd.cn

[R62] 找最占空间的文件
来源：http://fdh.316326.xyz

du -ah . | sort -rh | head -10
来源：http://vww.sysykeji.top

[R63] 内存与进程
来源：http://gsj.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://ydy.bjfxy.top

[R64] 结束进程
来源：http://nfj.smart0.xyz

kill -9 $(pgrep -f app.py)
来源：http://rif.fehbvm.com

[R65] 查看端口占用
来源：http://fzf.zhiwuduotai.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kgm.vehdjk.com

[R66] 定时任务
来源：http://qkk.dianchejie.cn

crontab -e;  crontab -l
来源：http://xnr.xylfe.cn

[R67] 生成随机十六进制串
来源：http://dnu.zdbjq.cn

openssl rand -hex 16
来源：http://rno.shuidangran.top

[R68] 计算文件校验值
来源：http://slv.zhaomingkeji.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://ecm.yfazqb.com

[R69] 生成随机密码
来源：http://bfl.cucudq.cn

head -c 16 /dev/urandom | base64
来源：http://gmm.sufxvd.cn

[R70] 时间戳与互转
来源：http://vff.fengsongda.top

date +%s;  date -d @1700000000
来源：http://xrz.9152youxi.cn

[R71] 日期格式化
来源：http://ant.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ahh.jqgfzy.top

[R72] 等待端口就绪
来源：http://hto.guowangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hjd.cqqwz.cn

[R73] 分割大日志
来源：http://nkt.xinyue.icu

split -l 1000 big.log part_
来源：http://zrl.ybcxt.top

[R74] 批量重命名
来源：http://ewn.hammf.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ygf.nwbrower.top

[R75] 导出环境变量
来源：http://pqn.jianghu66.top

export PATH="$HOME/bin:$PATH"
来源：http://oii.vqdsnc.cn

[R76] 使用临时文件
来源：http://eca.xuetiantiany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pdg.wangdashe.top

[R77] 读取用户输入
来源：http://umy.bbcook.cn

read -rp "请输入: " ans
来源：http://stm.hysaishi.cn

[R78] 交互式菜单
来源：http://wpk.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pey.shangyingyoupin.top

[R79] 解析命令行选项
来源：http://saa.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ovr.hammf.cn

[R80] 查看脚本执行耗时
来源：http://eus.fzhhl.top

time ./run.sh
来源：http://utt.sjlbkw.cn

================================================================================
来源：http://rtm.gogol.net.cn

S. C / C++ 专题
来源：http://wqu.yanxiufei.cn

================================================================================
来源：http://och.hcnkem.com

[S01] C：Hello World
来源：http://wyr.hesvh.cn

#include <stdio.h>
来源：http://xeq.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ssj.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://cgp.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://qyx.feifeiyinyue.top

[S03] C：读入整数
来源：http://bac.fengsongda.top

int x; scanf("%d", &x);
来源：http://blp.cqqwz.cn

[S04] C：字符串复制
来源：http://and.aibaodan.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vcz.zdqjudy.top

[S05] C：字符串长度
来源：http://tzp.yuxming.cn


<!-- 参考信息 -->