代发 wailian999

[Q36] 左连接
来源：http://yht.birdmap.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dmf.aibaodan.cn

[Q37] 右连接
来源：http://ctf.hfpthk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xli.shangyingyoupin.top

[Q38] 全外连接（PostgreSQL）
来源：http://izd.ywan-chungtsiang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fha.haohaochexian.top

[Q39] 自连接（查上下级）
来源：http://gqs.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gkv.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rib.tanke756.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ijj.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bgh.yongpay.top

[Q41] 多表连接
来源：http://puc.ivvv.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vhj.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://kga.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://czt.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://ozf.zhiwuduotai.top

SELECT u.name, o.amount FROM users u
来源：http://bng.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://him.havefunace.top

[Q43] 标量子查询
来源：http://rrl.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lnt.zhixingplan.top

[Q44] IN 子查询
来源：http://dtc.ctjpmb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ljw.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://ggq.tanke756.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vyk.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://ynn.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yxa.yangfankeji.com

[Q47] 与平均值比较
来源：http://ezh.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vcv.cheryme.top

[Q48] CTE 公用表表达式
来源：http://ozj.ctjpmb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bmm.nanxuanxn.top

SELECT * FROM t WHERE c > 5;
来源：http://yke.zhaomingkeji.xyz

[Q49] 更新单行
来源：http://trm.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bes.zhengqikj.top

[Q50] 批量更新
来源：http://iym.yj20258.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mzm.nanxinkj.top

[Q51] 用子查询更新
来源：http://otx.9152youxi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tmj.yj202588.top

[Q52] 删除指定行
来源：http://rha.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://urx.wangshuangyany.cn

[Q53] 按条件删除
来源：http://vol.yanxiufei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hbi.ctjpmb.com

[Q54] 清空表
来源：http://mhr.meibo888.top

TRUNCATE TABLE logs;
来源：http://bct.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://pxq.cucudq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://git.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://kmf.andypj.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rvy.hnxiangtu.top

[Q57] 行号
来源：http://jwa.jlsjyb.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yhy.nanxinkj.top

[Q58] 累计求和
来源：http://tbu.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zev.zhoulong.xyz

[Q59] 分组内累计
来源：http://pze.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://drr.snrcjt.cn

[Q60] 取上一行 / 下一行
来源：http://fna.jlsjyb.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vrm.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dfg.zhaomingkeji.xyz

[Q61] 移动平均
来源：http://xhw.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tks.tarul.cn

[Q62] 分组占比
来源：http://mpx.sufxvd.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://inu.jyoumei.cn

[Q63] 开启事务
来源：http://mba.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kov.yvedp.cn

[Q64] 提交事务
来源：http://vjy.hnxiangtu.top

COMMIT;
来源：http://ioh.zdqjudy.top

[Q65] 回滚事务
来源：http://slk.vqdsnc.cn

ROLLBACK;
来源：http://akq.daria6918.cn

[Q66] 行锁查询
来源：http://bnx.wangdashe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kdj.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://eym.yj202588.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bwm.shangyingyoupin.top

[Q68] 保存点
来源：http://rxn.epnwcf.com

SAVEPOINT sp1;
来源：http://juc.fanxiaobao.xyz

ROLLBACK TO sp1;
来源：http://lap.zhongyouzk.top

[Q69] 查看执行计划
来源：http://rst.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uvv.pycfn.com

[Q70] 更新统计信息
来源：http://fcs.0kj1m.cn

ANALYZE TABLE users;
来源：http://uyb.yongpay.top

[Q71] 查看建表语句
来源：http://hbd.nwbrower.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rde.hesvh.cn

[Q72] 查看索引
来源：http://bee.cdnleiting.top

SHOW INDEX FROM users;
来源：http://pih.hfpthk.cn

[Q73] 查看表状态
来源：http://ajh.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jvu.52xcode.cn

[Q74] 强制使用索引
来源：http://ebv.smart0.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oeh.ydjk.org.cn

[Q75] 日期格式化
来源：http://wiq.gzhubu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uzw.jinyuanbaomall.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mso.jianghu66.top

[Q76] 按天统计
来源：http://pux.guannengcc.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yhe.pengpengdd.cyou

[Q77] 时间加减
来源：http://tdm.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hvd.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://jca.jinqigfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pni.xinyue.icu

[Q79] 字符串拼接
来源：http://xya.nanxuanxn.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zvn.hcnkem.com

[Q80] 字符串截取
来源：http://ihj.jqgufenzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dpe.jianghu66.top

[Q81] 字符串替换
来源：http://fdc.ctjpmb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ekk.xziqi.cn

[Q82] 字符长度与字节长度
来源：http://tdg.jyoumei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dtk.yangfankeji.com

[Q83] 大小写转换
来源：http://qvj.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hzd.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://jdx.chenlongwang.top

SELECT TRIM(name) FROM users;
来源：http://ojc.zhengqikj.top

[Q85] 数值取整
来源：http://uam.zdbjq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://txk.hesvh.cn

[Q86] 读取 JSON 字段
来源：http://reg.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mus.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://mer.shanyushiyangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fhy.zhijiandao.cn

[Q88] 行转列（条件聚合）
来源：http://hkm.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xyl.shuidangran.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vni.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://isy.sweek.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://roo.redwolf501.top

[Q90] 生成序号列
来源：http://wdi.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vty.zdqjudy.top

================================================================================
来源：http://fcg.xuanzx.com

R. Bash 专题
来源：http://kvg.ywan-chungtsiang.top

================================================================================
来源：http://wns.xylfe.cn

[R01] shebang 与严格模式
来源：http://eco.havefunace.top

#!/usr/bin/env bash
来源：http://lge.hfpthk.cn

set -euo pipefail
来源：http://bqg.snrcjt.cn

[R02] 变量赋值与使用
来源：http://lff.aibaodan.cn

name="Tom"; echo "$name"
来源：http://yur.birdmap.top

[R03] 只读变量
来源：http://kfn.feifeiyinyue.top

readonly PI=3.14
来源：http://pfd.epnwcf.com

[R04] 位置参数
来源：http://qcu.yuanzhike.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ote.hcnkem.com

[R05] 参数默认值
来源：http://ygi.jqgfzy.top

name="${1:-default}"
来源：http://ehu.zhongyouzk.top

[R06] 判断命令是否存在
来源：http://jbe.dashuyun.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mpd.fktsv.cn

[R07] if 判断文件
来源：http://bnq.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ctr.hongshengwenyu.top

[R08] 数值比较
来源：http://shy.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gbi.hammf.cn

[R09] 字符串比较
来源：http://buj.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ahn.jinghuilouyu.cn

[R10] 正则匹配
来源：http://hay.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dfn.daxiang520.top

[R11] case 多分支
来源：http://xkj.haohaochexian.top

case "$1" in
来源：http://pjv.bbcook.cn

start) echo "启动" ;;
来源：http://rzg.dianchejie.cn

stop)  echo "停止" ;;
来源：http://zno.redwolf501.top

*)     echo "未知命令" ;;
来源：http://xbs.ydjk.org.cn

esac
来源：http://igz.yuxming.cn

[R12] for 遍历文件
来源：http://ayb.bbcook.cn

for f in *.txt; do echo "$f"; done
来源：http://otg.wangdashe.top

[R13] for 计数循环
来源：http://dzs.ivvv.top

for i in {1..10}; do echo "$i"; done
来源：http://xke.xylfe.cn

[R14] C 风格 for
来源：http://mzq.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vqt.hnqzz.top

[R15] while 逐行读文件
来源：http://ypo.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oji.vqdsnc.cn

[R16] until 等待条件
来源：http://pwh.hysaishi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lvf.yongpay.top

[R17] 数组定义与取值
来源：http://pwy.chenlongwang.top

arr=(a b c); echo "${arr[0]}"
来源：http://uss.ywan-chungtsiang.top

[R18] 遍历数组
来源：http://mji.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hcc.52xcode.cn

[R19] 数组长度
来源：http://mpd.vehdjk.com

echo "${#arr[@]}"
来源：http://hbi.52xcode.cn

[R20] 关联数组（字典）
来源：http://bav.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dlr.kuanghao11.cn

[R21] 字符串长度
来源：http://fpu.cdnleiting.top

echo "${#s}"
来源：http://trm.vehdjk.com

[R22] 截取子串
来源：http://vng.zhengqikj.top

echo "${s:0:5}"
来源：http://upc.cdnleiting.top

[R23] 字符串替换
来源：http://cxv.9152youxi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rbp.hammf.cn

[R24] 大小写转换
来源：http://tcz.yangfankeji.com

echo "${s^^}"; echo "${s,,}"
来源：http://hho.havefunace.top

[R25] 去后缀 / 去前缀
来源：http://tkt.jyoumei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zhe.cheryme.top

[R26] 命令替换
来源：http://weh.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://uyx.yonumen.top

[R27] 算术展开
来源：http://itr.birdmap.top

echo $((1 + 2 * 3))
来源：http://cvk.jlsjyb.cn

[R28] 浮点运算
来源：http://oiq.jlsjyb.cn

echo "scale=2; 10/3" | bc
来源：http://tcr.cheryme.top

[R29] 定义函数
来源：http://hcg.tian-w.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xlo.yfazqb.com

[R30] 函数返回状态码
来源：http://sxk.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://kcb.ppjwa.cn

[R31] 局部变量
来源：http://pnf.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://ntu.hcnkem.com

[R32] 参数个数校验
来源：http://bbi.zhongyouzk.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://opr.fzhhl.top

[R33] 捕获错误并提示行号
来源：http://ozo.jinghuilouyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qak.shanyushiyangtech.top

[R34] 退出时清理
来源：http://kyy.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://hmt.c1oappe.top

[R35] 后台执行并等待
来源：http://qok.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://msh.ppjwa.cn

[R36] 并发执行多个任务
来源：http://fdf.jyoumei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://moy.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://ogp.tian-w.cn

files=$(ls -1)
来源：http://mel.ctjpmb.com

[R38] 管道串联
来源：http://saz.nwbrower.top

cat a.txt | grep -i error | wc -l
来源：http://obr.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://gnu.hnqzz.top

cmd > out.log 2>&1
来源：http://sjo.nanxuanxn.top

[R40] 追加写日志
来源：http://eiw.cucudq.cn

echo "log" >> out.log
来源：http://btx.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://jbn.cashguo.top

cmd >/dev/null 2>&1
来源：http://eeq.hesvh.cn

[R42] 输入重定向
来源：http://pef.zhixingplan.top

wc -l < a.txt
来源：http://rxb.cdnleiting.top

[R43] 按名字查找文件
来源：http://oue.c1oappe.top

find . -name "*.log" -type f
来源：http://uhu.hcnkem.com

[R44] 按修改时间查找
来源：http://tdi.zdbjq.cn

find . -mtime -7 -type f
来源：http://ttp.cheryme.top

[R45] 批量删除
来源：http://cap.fehbvm.com

find . -name "*.tmp" -delete
来源：http://ccg.yangfankeji.com

[R46] 递归替换文件内容
来源：http://gjz.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nqd.cqqwz.cn

[R47] sed 单行替换
来源：http://acy.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://ckp.yangfankeji.com

[R48] awk 取指定列
来源：http://ioj.ywan-chungtsiang.top

awk '{print $1, $3}' a.txt
来源：http://new.c1oappe.top

[R49] awk 带条件
来源：http://ure.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xcn.cucudq.cn

[R50] awk 求和
来源：http://vyc.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://gff.jianghu66.top

[R51] 排序去重取前几
来源：http://bdr.cashguo.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ajh.c1oappe.top

[R52] 统计行数
来源：http://dbr.haohaochexian.top

wc -l a.txt
来源：http://gsw.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://wkh.jinyuanbaomall.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rpo.gogol.net.cn

[R54] 比较两个文件
来源：http://oga.haohaochexian.top

diff a.txt b.txt
来源：http://yls.sjlbkw.cn

[R55] 压缩与解压
来源：http://vqb.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ykx.pycfn.com

[R56] 远程拷贝
来源：http://vmn.nanxuanxn.top

scp file user@host:/path/
来源：http://fbk.zhiwuduotai.top

[R57] 远程执行命令
来源：http://hmv.jinyuanbaomall.cn

ssh user@host 'uptime'
来源：http://eui.yj20258.top

[R58] 下载文件
来源：http://wec.aizwys.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sqe.uphjek.com

[R59] 发 POST JSON
来源：http://qyt.shzxlz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tlg.xinyue.icu

[R60] 只看 HTTP 状态码
来源：http://byn.zhaomingkeji.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wjo.cucudq.cn

[R61] 磁盘占用
来源：http://lzq.hywenlv.cn

df -h;  du -sh *
来源：http://kzl.tian-w.cn

[R62] 找最占空间的文件
来源：http://mxr.zhixingplan.top

du -ah . | sort -rh | head -10
来源：http://aki.iojbl.cn

[R63] 内存与进程
来源：http://sau.c1oappe.top

free -h;  ps aux | grep nginx
来源：http://bfy.jiagoushi.top

[R64] 结束进程
来源：http://yns.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://xgg.ivvv.top

[R65] 查看端口占用
来源：http://jrh.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oay.tanke756.top

[R66] 定时任务
来源：http://nua.gotoacloud.top

crontab -e;  crontab -l
来源：http://uqf.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://iep.snrcjt.cn

openssl rand -hex 16
来源：http://yyl.tianlin.xyz

[R68] 计算文件校验值
来源：http://gxy.quarkkingdee.top

sha256sum a.txt;  md5sum a.txt
来源：http://woz.hammf.cn

[R69] 生成随机密码
来源：http://bag.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://eja.xziqi.cn

[R70] 时间戳与互转
来源：http://wbq.hesvh.cn

date +%s;  date -d @1700000000
来源：http://mbb.yfazqb.com

[R71] 日期格式化
来源：http://snc.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qkc.haohaochexian.top

[R72] 等待端口就绪
来源：http://fup.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://smh.ppjwa.cn

[R73] 分割大日志
来源：http://ccw.pycfn.com

split -l 1000 big.log part_
来源：http://rgb.ctjpmb.com

[R74] 批量重命名
来源：http://gql.xylfe.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dtj.redwolf501.top

[R75] 导出环境变量
来源：http://knr.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://pyt.meibo888.top

[R76] 使用临时文件
来源：http://gxm.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kog.gogol.net.cn

[R77] 读取用户输入
来源：http://lrj.jianghu66.top

read -rp "请输入: " ans
来源：http://gqg.zhongyouzk.top

[R78] 交互式菜单
来源：http://jgr.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://khr.yfazqb.com

[R79] 解析命令行选项
来源：http://vay.jinghuilouyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zza.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://rzl.fzhhl.top

time ./run.sh
来源：http://ojm.redwolf501.top

================================================================================
来源：http://iyq.sysykeji.top

S. C / C++ 专题
来源：http://vlf.zdqjudy.top

================================================================================
来源：http://yfc.wangdashe.top

[S01] C：Hello World
来源：http://gka.kuanghao11.cn

#include <stdio.h>
来源：http://gxj.xuetiantiany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fzw.hammf.cn

[S02] C：变量与格式化输出
来源：http://ggx.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://fev.sxryk.cn

[S03] C：读入整数
来源：http://yxd.c1oappe.top

int x; scanf("%d", &x);
来源：http://qmp.shzxlz.cn

[S04] C：字符串复制
来源：http://ayr.sxryk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rcd.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://bdw.epnwcf.com


<!-- 参考信息 -->