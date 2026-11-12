代发 wailian999

[Q36] 左连接
来源：http://uwj.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cum.hongshengwenyu.top

[Q37] 右连接
来源：http://yvi.shangyingyoupin.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://msv.xuanzx.com

[Q38] 全外连接（PostgreSQL）
来源：http://uee.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vzq.epnwcf.com

[Q39] 自连接（查上下级）
来源：http://mbf.ivvv.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hgs.cashguo.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qxn.xinyue.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://xap.daxiang520.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fwe.ywan-chungtsiang.top

[Q41] 多表连接
来源：http://mzf.ehwqpu.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://snu.vqdsnc.cn

JOIN users u ON u.id = o.user_id
来源：http://dgz.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://cus.hywenlv.cn

[Q42] 连接条件附加过滤
来源：http://int.dianchejie.cn

SELECT u.name, o.amount FROM users u
来源：http://wfd.ctjpmb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vou.316326.xyz

[Q43] 标量子查询
来源：http://gim.ydzc1.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://duz.zdqjudy.top

[Q44] IN 子查询
来源：http://nlr.redwolf501.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dmk.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://inu.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dsb.jinqigufen.top

[Q46] NOT EXISTS 判断不存在
来源：http://rll.jqgufenzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jca.zhaomingkeji.xyz

[Q47] 与平均值比较
来源：http://alk.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gzb.sjlbkw.cn

[Q48] CTE 公用表表达式
来源：http://qss.wangshuangyany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ngf.tian-w.cn

SELECT * FROM t WHERE c > 5;
来源：http://mvt.zhiwuduotai.top

[Q49] 更新单行
来源：http://xum.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zia.sysykeji.top

[Q50] 批量更新
来源：http://qpi.guowangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zva.cqqwz.cn

[Q51] 用子查询更新
来源：http://exf.fanxiaobao.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rvl.xziqi.cn

[Q52] 删除指定行
来源：http://acv.zhiwuduotai.top

DELETE FROM users WHERE id = 10;
来源：http://qhf.ppjwa.cn

[Q53] 按条件删除
来源：http://qvi.fanxiaobao.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vbl.jinghuilouyu.cn

[Q54] 清空表
来源：http://bue.zhiwuduotai.top

TRUNCATE TABLE logs;
来源：http://mpv.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://mnd.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nug.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://uii.havefunace.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rgc.guowangkeji.top

[Q57] 行号
来源：http://pmg.bbcook.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wyr.dianchejie.cn

[Q58] 累计求和
来源：http://jpo.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yjz.chenzaomai.com

[Q59] 分组内累计
来源：http://yiy.guowangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jpo.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://mpy.ivvv.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yyg.daxiang520.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tye.gzhubu.top

[Q61] 移动平均
来源：http://vmg.hywenlv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lyt.chenzaomai.com

[Q62] 分组占比
来源：http://oal.yanxiufei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ooz.jyoumei.cn

[Q63] 开启事务
来源：http://jlh.redwolf501.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sqp.iojbl.cn

[Q64] 提交事务
来源：http://ctd.hfpthk.cn

COMMIT;
来源：http://mpj.bjfxy.top

[Q65] 回滚事务
来源：http://upp.yanxiufei.cn

ROLLBACK;
来源：http://xoa.bjfxy.top

[Q66] 行锁查询
来源：http://aoi.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yre.yanxiufei.cn

[Q67] 设置隔离级别
来源：http://wai.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yka.gogol.net.cn

[Q68] 保存点
来源：http://zln.nanxuanxn.top

SAVEPOINT sp1;
来源：http://ljw.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://sey.guannengcc.top

[Q69] 查看执行计划
来源：http://cce.cucudq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ooq.wangshuangyany.cn

[Q70] 更新统计信息
来源：http://gfa.shuidangran.top

ANALYZE TABLE users;
来源：http://wrd.gzhubu.top

[Q71] 查看建表语句
来源：http://fgq.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hzt.gzhubu.top

[Q72] 查看索引
来源：http://hum.yuxming.cn

SHOW INDEX FROM users;
来源：http://lpp.shanyushiyangkeji.top

[Q73] 查看表状态
来源：http://lxe.yueranfly.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ypr.ctjpmb.com

[Q74] 强制使用索引
来源：http://dqw.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hoc.yueranfly.top

[Q75] 日期格式化
来源：http://xzw.tanke756.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eef.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://frz.zhaomingkeji.xyz

[Q76] 按天统计
来源：http://rjt.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yrm.svipenyu.cn

[Q77] 时间加减
来源：http://xwr.yj20258.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lkd.ppjwa.cn

[Q78] 当前时间
来源：http://olv.wangshuangyany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kwd.hcnkem.com

[Q79] 字符串拼接
来源：http://bjr.pengpengdd.cyou

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xlj.jinyuanbaomall.cn

[Q80] 字符串截取
来源：http://mtk.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iod.fengsongda.top

[Q81] 字符串替换
来源：http://ssd.shangyingyoupin.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://edn.ybcxt.top

[Q82] 字符长度与字节长度
来源：http://bdw.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://een.tanke756.top

[Q83] 大小写转换
来源：http://lrn.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mcb.daxiang520.top

[Q84] 去除首尾空格
来源：http://bmb.jqgufenzy.top

SELECT TRIM(name) FROM users;
来源：http://akf.fzhhl.top

[Q85] 数值取整
来源：http://guu.kuanghao11.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ydq.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://kps.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zyp.ctjpmb.com

[Q87] JSON 字段做条件
来源：http://eid.jlsjyb.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jgl.cqqwz.cn

[Q88] 行转列（条件聚合）
来源：http://cfq.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qve.sxryk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vsr.hcnkem.com

[Q89] 判断表是否存在
来源：http://vej.fengsongda.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ndm.yj20258.top

[Q90] 生成序号列
来源：http://fee.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ato.xuanzx.com

================================================================================
来源：http://yxw.chenjidiqi.icu

R. Bash 专题
来源：http://trx.c1oappe.top

================================================================================
来源：http://ahw.hesvh.cn

[R01] shebang 与严格模式
来源：http://myu.ppjwa.cn

#!/usr/bin/env bash
来源：http://cuv.cheryme.top

set -euo pipefail
来源：http://ygp.xinyue.icu

[R02] 变量赋值与使用
来源：http://epq.hnqzz.top

name="Tom"; echo "$name"
来源：http://alg.cqqwz.cn

[R03] 只读变量
来源：http://dkx.bbcook.cn

readonly PI=3.14
来源：http://vpk.meibo888.top

[R04] 位置参数
来源：http://mjf.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xnj.hnxiangtu.top

[R05] 参数默认值
来源：http://hqw.tian-w.cn

name="${1:-default}"
来源：http://fis.sweek.top

[R06] 判断命令是否存在
来源：http://cow.ehwqpu.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cxk.yanxiufei.cn

[R07] if 判断文件
来源：http://vrm.gotoacloud.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lsg.ehwqpu.com

[R08] 数值比较
来源：http://jsd.cdnleiting.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qsy.aibaodan.cn

[R09] 字符串比较
来源：http://rtb.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bcf.feifeiyinyue.top

[R10] 正则匹配
来源：http://tum.zhengqikj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cnb.cheryme.top

[R11] case 多分支
来源：http://asz.hfpthk.cn

case "$1" in
来源：http://zqf.sxryk.cn

start) echo "启动" ;;
来源：http://ycz.epnwcf.com

stop)  echo "停止" ;;
来源：http://mxz.zhongyouzk.top

*)     echo "未知命令" ;;
来源：http://apb.dashuyun.cn

esac
来源：http://uni.andypj.xyz

[R12] for 遍历文件
来源：http://nft.cdnleiting.top

for f in *.txt; do echo "$f"; done
来源：http://dly.yanxiufei.cn

[R13] for 计数循环
来源：http://fih.shanyushiyangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://fyh.sxryk.cn

[R14] C 风格 for
来源：http://ybs.yj20258888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wqa.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://fsz.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dcn.xinyue.icu

[R16] until 等待条件
来源：http://axk.ywan-chungtsiang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lxw.yongpay.top

[R17] 数组定义与取值
来源：http://vvr.zhijiandao.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pyr.yj202588.top

[R18] 遍历数组
来源：http://mrj.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ayr.guowangkeji.top

[R19] 数组长度
来源：http://rna.svipenyu.cn

echo "${#arr[@]}"
来源：http://bhr.smart0.xyz

[R20] 关联数组（字典）
来源：http://cmz.quarkkingdee.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ygs.hysaishi.cn

[R21] 字符串长度
来源：http://gwh.jiagoushi.top

echo "${#s}"
来源：http://vld.jqgufenzy.top

[R22] 截取子串
来源：http://obm.fengsongda.top

echo "${s:0:5}"
来源：http://jsa.52xcode.cn

[R23] 字符串替换
来源：http://sol.ppjwa.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tvy.fehbvm.com

[R24] 大小写转换
来源：http://gfj.hfpthk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://msh.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://aqr.xziqi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bgw.xylfe.cn

[R26] 命令替换
来源：http://zsh.jqgufenzy.top

now=$(date +%F); echo "$now"
来源：http://aqw.zhixingplan.top

[R27] 算术展开
来源：http://ywt.nwbrower.top

echo $((1 + 2 * 3))
来源：http://hfy.daxiang520.top

[R28] 浮点运算
来源：http://mfb.feifeiyinyue.top

echo "scale=2; 10/3" | bc
来源：http://xta.hammf.cn

[R29] 定义函数
来源：http://ssm.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fwn.hesvh.cn

[R30] 函数返回状态码
来源：http://loy.xingfuxueyuan.xyz

f() { return 0; }; f || echo "失败了"
来源：http://crf.bjfxy.top

[R31] 局部变量
来源：http://oxz.316326.xyz

f() { local x=1; echo "$x"; }
来源：http://xfa.sufxvd.cn

[R32] 参数个数校验
来源：http://vlr.cdnleiting.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://abj.yanxiufei.cn

[R33] 捕获错误并提示行号
来源：http://slw.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bkc.epnwcf.com

[R34] 退出时清理
来源：http://mxg.guowangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://hic.zhoulong.xyz

[R35] 后台执行并等待
来源：http://iih.zdqjudy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fjx.nanxuanxn.top

[R36] 并发执行多个任务
来源：http://zwa.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://luc.svipenyu.cn

[R37] 把输出赋给变量
来源：http://kdf.guowangkeji.top

files=$(ls -1)
来源：http://vlk.zhiwuduotai.top

[R38] 管道串联
来源：http://ajb.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://bna.zhoulong.xyz

[R39] 重定向标准输出与错误
来源：http://nwt.jiagoushi.top

cmd > out.log 2>&1
来源：http://iwh.hongshengwenyu.top

[R40] 追加写日志
来源：http://pmv.yangfankeji.com

echo "log" >> out.log
来源：http://rvn.shzxlz.cn

[R41] 丢弃输出
来源：http://ark.jinghuilouyu.cn

cmd >/dev/null 2>&1
来源：http://ldi.sxryk.cn

[R42] 输入重定向
来源：http://lbp.xinyue.icu

wc -l < a.txt
来源：http://anr.daria6918.cn

[R43] 按名字查找文件
来源：http://lmj.dashuyun.cn

find . -name "*.log" -type f
来源：http://kqy.dianchejie.cn

[R44] 按修改时间查找
来源：http://dtc.zhongyouzk.top

find . -mtime -7 -type f
来源：http://apo.jlsjyb.cn

[R45] 批量删除
来源：http://cuw.pycfn.com

find . -name "*.tmp" -delete
来源：http://fzg.nwbrower.top

[R46] 递归替换文件内容
来源：http://owu.shanyushiyangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rye.aizwys.cn

[R47] sed 单行替换
来源：http://cek.hnxiangtu.top

sed -i 's/foo/bar/g' a.txt
来源：http://ifk.haohaochexian.top

[R48] awk 取指定列
来源：http://lrb.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://yhx.xuanzx.com

[R49] awk 带条件
来源：http://tcl.hysaishi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rit.ppjwa.cn

[R50] awk 求和
来源：http://dal.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://iqy.daxiang520.top

[R51] 排序去重取前几
来源：http://avl.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mht.birdmap.top

[R52] 统计行数
来源：http://qbi.ctjpmb.com

wc -l a.txt
来源：http://zxd.shangyingyoupin.top

[R53] 查看文件头与实时尾
来源：http://tyv.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iiw.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://ayv.wangshuangyany.cn

diff a.txt b.txt
来源：http://dpv.shangyingyoupin.top

[R55] 压缩与解压
来源：http://xyh.vqdsnc.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wwg.yanxiufei.cn

[R56] 远程拷贝
来源：http://vyd.yj20258888.top

scp file user@host:/path/
来源：http://oly.chenlongwang.top

[R57] 远程执行命令
来源：http://eqw.nanxinkj.top

ssh user@host 'uptime'
来源：http://xus.snrcjt.cn

[R58] 下载文件
来源：http://wdb.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jzp.jiagoushi.top

[R59] 发 POST JSON
来源：http://yxx.vehdjk.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ver.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://ong.yj20258.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jla.haohaochexian.top

[R61] 磁盘占用
来源：http://com.zdbjq.cn

df -h;  du -sh *
来源：http://rjz.svipenyu.cn

[R62] 找最占空间的文件
来源：http://xee.ppjwa.cn

du -ah . | sort -rh | head -10
来源：http://kmz.chenjidiqi.icu

[R63] 内存与进程
来源：http://bzi.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://dql.52xcode.cn

[R64] 结束进程
来源：http://lbh.zhiwuduotai.top

kill -9 $(pgrep -f app.py)
来源：http://rgb.jqgufenzy.top

[R65] 查看端口占用
来源：http://jqc.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://imo.fanxiaobao.xyz

[R66] 定时任务
来源：http://ecm.ivvv.top

crontab -e;  crontab -l
来源：http://scw.ppjwa.cn

[R67] 生成随机十六进制串
来源：http://ufc.0kj1m.cn

openssl rand -hex 16
来源：http://yog.0kj1m.cn

[R68] 计算文件校验值
来源：http://qws.quarkkingdee.top

sha256sum a.txt;  md5sum a.txt
来源：http://oox.dianchejie.cn

[R69] 生成随机密码
来源：http://kkv.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://vtp.cheryme.top

[R70] 时间戳与互转
来源：http://nzw.hongshengwenyu.top

date +%s;  date -d @1700000000
来源：http://tqu.fengsongda.top

[R71] 日期格式化
来源：http://zvu.sysykeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wst.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://hkf.sweek.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mzp.jqgfzy.top

[R73] 分割大日志
来源：http://vgy.hnqzz.top

split -l 1000 big.log part_
来源：http://otr.yangfankeji.com

[R74] 批量重命名
来源：http://kwh.smart0.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jqr.tian-w.cn

[R75] 导出环境变量
来源：http://sex.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://kju.hysaishi.cn

[R76] 使用临时文件
来源：http://dvc.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xfq.ydjk.org.cn

[R77] 读取用户输入
来源：http://ned.zhaomingkeji.xyz

read -rp "请输入: " ans
来源：http://nhq.tianlin.xyz

[R78] 交互式菜单
来源：http://rvw.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zyu.tianlin.xyz

[R79] 解析命令行选项
来源：http://rnt.yongpay.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kwp.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://siy.jyoumei.cn

time ./run.sh
来源：http://bly.meibo888.top

================================================================================
来源：http://bsn.meibo888.top

S. C / C++ 专题
来源：http://lup.bbcook.cn

================================================================================
来源：http://ust.0kj1m.cn

[S01] C：Hello World
来源：http://kzk.ydzc1.top

#include <stdio.h>
来源：http://gfv.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mha.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://mpu.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://eyr.aizwys.cn

[S03] C：读入整数
来源：http://xlu.xuanzx.com

int x; scanf("%d", &x);
来源：http://bmc.jinqigufen.top

[S04] C：字符串复制
来源：http://mxo.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://agk.ctjpmb.com

[S05] C：字符串长度
来源：http://bwx.shzxlz.cn


<!-- 参考信息 -->