代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kdo.shuidangran.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xgu.xinyue.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jzw.yj20258.top

[Q41] 多表连接
来源：http://kul.andypj.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://uwf.shangyingyoupin.top

JOIN users u ON u.id = o.user_id
来源：http://kmb.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://euh.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://tda.chenzaomai.com

SELECT u.name, o.amount FROM users u
来源：http://nuo.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kcn.zdqjudy.top

[Q43] 标量子查询
来源：http://sti.sxryk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rvr.shangyingyoupin.top

[Q44] IN 子查询
来源：http://hgs.yanxiufei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://txq.ppjwa.cn

[Q45] EXISTS 判断存在
来源：http://flj.jinghuilouyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kcu.jyoumei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nsp.zhongyouzk.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vwf.guowangkeji.top

[Q47] 与平均值比较
来源：http://pkh.mhx1999.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mzm.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://qlb.epnwcf.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mfu.cheryme.top

SELECT * FROM t WHERE c > 5;
来源：http://qxl.dashuyun.cn

[Q49] 更新单行
来源：http://dcv.nwbrower.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fav.shanyushiyangkeji.top

[Q50] 批量更新
来源：http://txo.hnxiangtu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gdj.yj202588.top

[Q51] 用子查询更新
来源：http://gvh.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zac.zhengqikj.top

[Q52] 删除指定行
来源：http://ugq.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://nnq.cucudq.cn

[Q53] 按条件删除
来源：http://azb.guannengcc.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fxr.gzhubu.top

[Q54] 清空表
来源：http://csf.jqgufenzy.top

TRUNCATE TABLE logs;
来源：http://dop.hammf.cn

[Q55] 排名（并列占位）
来源：http://jxs.yueranfly.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aqh.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://byr.zhoulong.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ztf.shanyushiyangkeji.top

[Q57] 行号
来源：http://tyc.vqdsnc.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lti.tianlin.xyz

[Q58] 累计求和
来源：http://knn.guowangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gtf.xziqi.cn

[Q59] 分组内累计
来源：http://nls.jlsjyb.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ehc.uphjek.com

[Q60] 取上一行 / 下一行
来源：http://mpw.xuetiantiany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ntc.shanyushiyangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bgr.zycfv.cn

[Q61] 移动平均
来源：http://kqm.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://grc.uphjek.com

[Q62] 分组占比
来源：http://rra.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://irj.shuidangran.top

[Q63] 开启事务
来源：http://tyq.quarkkingdee.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dol.hnqzz.top

[Q64] 提交事务
来源：http://cfh.hywenlv.cn

COMMIT;
来源：http://jzg.ydzc1.top

[Q65] 回滚事务
来源：http://bov.zhoulong.xyz

ROLLBACK;
来源：http://wys.yvedp.cn

[Q66] 行锁查询
来源：http://vcl.kuanghao11.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hhe.jlsjyb.cn

[Q67] 设置隔离级别
来源：http://qep.tian-w.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wha.andypj.xyz

[Q68] 保存点
来源：http://qli.mhx1999.top

SAVEPOINT sp1;
来源：http://wgt.shanyushiyangkeji.top

ROLLBACK TO sp1;
来源：http://pfq.xuanzx.com

[Q69] 查看执行计划
来源：http://uyi.gaohongyu789.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jro.ppjwa.cn

[Q70] 更新统计信息
来源：http://rzj.snrcjt.cn

ANALYZE TABLE users;
来源：http://jem.snrcjt.cn

[Q71] 查看建表语句
来源：http://vzd.daria6918.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hvt.cqqwz.cn

[Q72] 查看索引
来源：http://ddm.bbcook.cn

SHOW INDEX FROM users;
来源：http://xef.hysaishi.cn

[Q73] 查看表状态
来源：http://ejt.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nun.aibaodan.cn

[Q74] 强制使用索引
来源：http://kma.aibaodan.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wym.hywenlv.cn

[Q75] 日期格式化
来源：http://kgl.zhijiandao.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xxm.shuidangran.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nzp.zhiwuduotai.top

[Q76] 按天统计
来源：http://ony.xuetiantiany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://raz.redwolf501.top

[Q77] 时间加减
来源：http://def.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qdo.fehbvm.com

[Q78] 当前时间
来源：http://jrr.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uqp.jinyuanbaomall.cn

[Q79] 字符串拼接
来源：http://mzn.fktsv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qnx.shanyushiyangkeji.top

[Q80] 字符串截取
来源：http://tse.jlsjyb.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pxf.sysykeji.top

[Q81] 字符串替换
来源：http://pzs.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://muc.yj20258.top

[Q82] 字符长度与字节长度
来源：http://qdw.yj20258888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ctu.wangshuangyany.cn

[Q83] 大小写转换
来源：http://fmy.zdqjudy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ghm.ybcxt.top

[Q84] 去除首尾空格
来源：http://vgz.jqgfzy.top

SELECT TRIM(name) FROM users;
来源：http://ntn.sweek.top

[Q85] 数值取整
来源：http://lkr.vehdjk.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nhu.yonumen.top

[Q86] 读取 JSON 字段
来源：http://oab.snrcjt.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bel.sxryk.cn

[Q87] JSON 字段做条件
来源：http://awu.shuidangran.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qic.chenzaomai.com

[Q88] 行转列（条件聚合）
来源：http://zul.daxiang520.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nze.hongshengwenyu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fhc.ctjpmb.com

[Q89] 判断表是否存在
来源：http://wzc.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iso.hesvh.cn

[Q90] 生成序号列
来源：http://uei.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kaz.haohaochexian.top

================================================================================
来源：http://nji.sufxvd.cn

R. Bash 专题
来源：http://rfq.svipenyu.cn

================================================================================
来源：http://wln.gotoacloud.top

[R01] shebang 与严格模式
来源：http://kws.shanyushiyangtech.top

#!/usr/bin/env bash
来源：http://piz.cashguo.top

set -euo pipefail
来源：http://fki.daxiang520.top

[R02] 变量赋值与使用
来源：http://agt.hnqzz.top

name="Tom"; echo "$name"
来源：http://ieg.ydjk.org.cn

[R03] 只读变量
来源：http://chb.hongshengwenyu.top

readonly PI=3.14
来源：http://fmg.hfpthk.cn

[R04] 位置参数
来源：http://vud.sysykeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wvr.hammf.cn

[R05] 参数默认值
来源：http://flh.guowangkeji.top

name="${1:-default}"
来源：http://mle.chenzaomai.com

[R06] 判断命令是否存在
来源：http://tfi.ydzc1.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wha.tian-w.cn

[R07] if 判断文件
来源：http://ccc.xylfe.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yob.guannengcc.top

[R08] 数值比较
来源：http://vcm.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mvp.ehwqpu.com

[R09] 字符串比较
来源：http://awj.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fcl.52xcode.cn

[R10] 正则匹配
来源：http://skr.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nhl.meibo888.top

[R11] case 多分支
来源：http://ftu.hammf.cn

case "$1" in
来源：http://vzw.cucudq.cn

start) echo "启动" ;;
来源：http://ogi.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://lvx.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://xae.epnwcf.com

esac
来源：http://icj.gzhubu.top

[R12] for 遍历文件
来源：http://rjw.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://cqt.hfpthk.cn

[R13] for 计数循环
来源：http://zds.tianlin.xyz

for i in {1..10}; do echo "$i"; done
来源：http://cxe.hywenlv.cn

[R14] C 风格 for
来源：http://jve.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wyo.tianlin.xyz

[R15] while 逐行读文件
来源：http://riv.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zkx.aizwys.cn

[R16] until 等待条件
来源：http://nlh.aizwys.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fcn.pycfn.com

[R17] 数组定义与取值
来源：http://ewy.gotoacloud.top

arr=(a b c); echo "${arr[0]}"
来源：http://xgq.sweek.top

[R18] 遍历数组
来源：http://hio.hysaishi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mie.yangfankeji.com

[R19] 数组长度
来源：http://jpg.yuxming.cn

echo "${#arr[@]}"
来源：http://mlu.sufxvd.cn

[R20] 关联数组（字典）
来源：http://azg.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jpw.tian-w.cn

[R21] 字符串长度
来源：http://iir.ppjwa.cn

echo "${#s}"
来源：http://ubh.hfpthk.cn

[R22] 截取子串
来源：http://gsq.sweek.top

echo "${s:0:5}"
来源：http://hoo.yj202588.top

[R23] 字符串替换
来源：http://hqq.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ext.yuanzhike.top

[R24] 大小写转换
来源：http://jaz.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://dyi.zycfv.cn

[R25] 去后缀 / 去前缀
来源：http://eax.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://jzm.0kj1m.cn

[R26] 命令替换
来源：http://lsu.shuidangran.top

now=$(date +%F); echo "$now"
来源：http://bfb.hnqzz.top

[R27] 算术展开
来源：http://kvk.tian-w.cn

echo $((1 + 2 * 3))
来源：http://nxs.svipenyu.cn

[R28] 浮点运算
来源：http://zdg.feifeiyinyue.top

echo "scale=2; 10/3" | bc
来源：http://osb.gotoacloud.top

[R29] 定义函数
来源：http://cak.shangyingyoupin.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rzv.yj20258.top

[R30] 函数返回状态码
来源：http://weu.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://pwf.xziqi.cn

[R31] 局部变量
来源：http://wdz.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://own.zhiwuduotai.top

[R32] 参数个数校验
来源：http://xrl.jinghuilouyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jyf.shzxlz.cn

[R33] 捕获错误并提示行号
来源：http://yqc.fktsv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vqc.fehbvm.com

[R34] 退出时清理
来源：http://fru.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://idf.zhixingplan.top

[R35] 后台执行并等待
来源：http://wsz.jinyuanbaomall.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mby.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://joy.hammf.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mzi.fanxiaobao.xyz

[R37] 把输出赋给变量
来源：http://oat.fzhhl.top

files=$(ls -1)
来源：http://zhq.bjfxy.top

[R38] 管道串联
来源：http://wfc.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://ypw.hongshengwenyu.top

[R39] 重定向标准输出与错误
来源：http://csy.wangdashe.top

cmd > out.log 2>&1
来源：http://hic.sufxvd.cn

[R40] 追加写日志
来源：http://rur.jinqigufen.top

echo "log" >> out.log
来源：http://mkb.havefunace.top

[R41] 丢弃输出
来源：http://onb.xziqi.cn

cmd >/dev/null 2>&1
来源：http://oho.gotoacloud.top

[R42] 输入重定向
来源：http://kvo.nanxinkj.top

wc -l < a.txt
来源：http://qck.jianghu66.top

[R43] 按名字查找文件
来源：http://ait.chenzaomai.com

find . -name "*.log" -type f
来源：http://cae.yongpay.top

[R44] 按修改时间查找
来源：http://lvf.chenjidiqi.icu

find . -mtime -7 -type f
来源：http://nlx.fzhhl.top

[R45] 批量删除
来源：http://pxc.redwolf501.top

find . -name "*.tmp" -delete
来源：http://pmb.snrcjt.cn

[R46] 递归替换文件内容
来源：http://emb.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bgt.svipenyu.cn

[R47] sed 单行替换
来源：http://jma.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://kqu.nanxuanxn.top

[R48] awk 取指定列
来源：http://mfz.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://nyk.jianghu66.top

[R49] awk 带条件
来源：http://szy.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jnx.0kj1m.cn

[R50] awk 求和
来源：http://jtg.tarul.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ljc.svipenyu.cn

[R51] 排序去重取前几
来源：http://bog.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hon.hnqzz.top

[R52] 统计行数
来源：http://ujs.zhaomingkeji.xyz

wc -l a.txt
来源：http://ayl.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://alq.hysaishi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fmy.dashuyun.cn

[R54] 比较两个文件
来源：http://cao.yj202588.top

diff a.txt b.txt
来源：http://omv.zhongyouzk.top

[R55] 压缩与解压
来源：http://nre.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ilg.cqqwz.cn

[R56] 远程拷贝
来源：http://kkf.zhongyouzk.top

scp file user@host:/path/
来源：http://cqc.ctjpmb.com

[R57] 远程执行命令
来源：http://ilx.ehwqpu.com

ssh user@host 'uptime'
来源：http://uqm.yanxiufei.cn

[R58] 下载文件
来源：http://tue.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mzn.zhijiandao.cn

[R59] 发 POST JSON
来源：http://nyo.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vjj.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://dfc.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gcc.ppjwa.cn

[R61] 磁盘占用
来源：http://vnv.hcnkem.com

df -h;  du -sh *
来源：http://akg.yj20258.top

[R62] 找最占空间的文件
来源：http://ofh.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://xhe.wangdashe.top

[R63] 内存与进程
来源：http://ner.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://wht.yfazqb.com

[R64] 结束进程
来源：http://mat.yj20258.top

kill -9 $(pgrep -f app.py)
来源：http://sbb.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://jqu.meibo888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hoc.gogol.net.cn

[R66] 定时任务
来源：http://xuo.xinyue.icu

crontab -e;  crontab -l
来源：http://yye.ybcxt.top

[R67] 生成随机十六进制串
来源：http://zes.zhixingplan.top

openssl rand -hex 16
来源：http://kjh.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://lwd.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jte.nanxuanxn.top

[R69] 生成随机密码
来源：http://ogx.gzhubu.top

head -c 16 /dev/urandom | base64
来源：http://ecg.wangdashe.top

[R70] 时间戳与互转
来源：http://azd.xylfe.cn

date +%s;  date -d @1700000000
来源：http://icl.birdmap.top

[R71] 日期格式化
来源：http://wfy.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lrl.nanxuanxn.top

[R72] 等待端口就绪
来源：http://gla.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://awx.fengsongda.top

[R73] 分割大日志
来源：http://zoa.redwolf501.top

split -l 1000 big.log part_
来源：http://kra.ppjwa.cn

[R74] 批量重命名
来源：http://hid.jinyuanbaomall.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://teq.jianghu66.top

[R75] 导出环境变量
来源：http://duw.mhx1999.top

export PATH="$HOME/bin:$PATH"
来源：http://slm.chenlongwang.top

[R76] 使用临时文件
来源：http://xxn.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dgr.yonumen.top

[R77] 读取用户输入
来源：http://xwo.cheryme.top

read -rp "请输入: " ans
来源：http://mlc.gotoacloud.top

[R78] 交互式菜单
来源：http://pdz.daria6918.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cxs.ctjpmb.com

[R79] 解析命令行选项
来源：http://yfw.xuetiantiany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eoo.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://okb.9152youxi.cn

time ./run.sh
来源：http://zio.chenjidiqi.icu

================================================================================
来源：http://qhv.snrcjt.cn

S. C / C++ 专题
来源：http://cfl.zycfv.cn

================================================================================
来源：http://igq.hfpthk.cn

[S01] C：Hello World
来源：http://edd.smart0.xyz

#include <stdio.h>
来源：http://eou.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://qlh.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://oim.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://qxi.chenzaomai.com

[S03] C：读入整数
来源：http://hea.tian-w.cn

int x; scanf("%d", &x);
来源：http://lxi.0kj1m.cn

[S04] C：字符串复制
来源：http://rlg.zhaomingkeji.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://ayl.tarul.cn

[S05] C：字符串长度
来源：http://ulm.sweek.top

strlen(s)
来源：http://vpt.yj202588.top

[S06] C：字符串比较
来源：http://mil.sysykeji.top

strcmp(a, b) == 0
来源：http://ype.dashuyun.cn

[S07] C：数组遍历求和
来源：http://jql.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vdp.hysaishi.cn

[S08] C：动态内存分配与释放
来源：http://qje.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yzm.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://xvn.shuidangran.top


<!-- 参考信息 -->