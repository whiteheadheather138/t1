代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://pld.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gdo.xuanzx.com

[Q39] 自连接（查上下级）
来源：http://xkp.snrcjt.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tbl.smart0.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fcb.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://sif.cheryme.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vao.guowangkeji.top

[Q41] 多表连接
来源：http://oqd.havefunace.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mtu.gzhubu.top

JOIN users u ON u.id = o.user_id
来源：http://bnn.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://jrl.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://jwa.xuetiantiany.cn

SELECT u.name, o.amount FROM users u
来源：http://zej.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ima.aizwys.cn

[Q43] 标量子查询
来源：http://cii.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aql.ctjpmb.com

[Q44] IN 子查询
来源：http://kuk.hongshengwenyu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bzt.wangdashe.top

[Q45] EXISTS 判断存在
来源：http://fyx.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://goa.hnqzz.top

[Q46] NOT EXISTS 判断不存在
来源：http://zks.yangfankeji.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pdh.9152youxi.cn

[Q47] 与平均值比较
来源：http://ogq.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vua.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://zsg.zdqjudy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zju.xuanzx.com

SELECT * FROM t WHERE c > 5;
来源：http://tyx.jinghuilouyu.cn

[Q49] 更新单行
来源：http://dua.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nka.ybcxt.top

[Q50] 批量更新
来源：http://slx.birdmap.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zxn.xuanzx.com

[Q51] 用子查询更新
来源：http://saw.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zpp.nwbrower.top

[Q52] 删除指定行
来源：http://dxl.xuanzx.com

DELETE FROM users WHERE id = 10;
来源：http://plm.redwolf501.top

[Q53] 按条件删除
来源：http://ape.hysaishi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rcq.hfpthk.cn

[Q54] 清空表
来源：http://bbi.xylfe.cn

TRUNCATE TABLE logs;
来源：http://tkx.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://ehx.mhx1999.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gae.jinqigufen.top

[Q56] 密集排名（并列不占位）
来源：http://wmn.redwolf501.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oor.yangfankeji.com

[Q57] 行号
来源：http://cig.hnqzz.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sno.jinghuilouyu.cn

[Q58] 累计求和
来源：http://khl.ywan-chungtsiang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pzg.tarul.cn

[Q59] 分组内累计
来源：http://aza.kuanghao11.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uvj.wangdashe.top

[Q60] 取上一行 / 下一行
来源：http://pwy.tianlin.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bjs.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uny.aibaodan.cn

[Q61] 移动平均
来源：http://hex.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dfv.andypj.xyz

[Q62] 分组占比
来源：http://kxy.yongpay.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lmf.9152youxi.cn

[Q63] 开启事务
来源：http://rzy.meibo888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://cut.nanxinkj.top

[Q64] 提交事务
来源：http://fls.jinqigfzy.top

COMMIT;
来源：http://gqs.zhixingplan.top

[Q65] 回滚事务
来源：http://oug.jqgufenzy.top

ROLLBACK;
来源：http://yxx.feifeiyinyue.top

[Q66] 行锁查询
来源：http://krh.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wrs.zhiwuduotai.top

[Q67] 设置隔离级别
来源：http://dip.hysaishi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hlx.yueranfly.top

[Q68] 保存点
来源：http://dhi.zdqjudy.top

SAVEPOINT sp1;
来源：http://bim.yfazqb.com

ROLLBACK TO sp1;
来源：http://gzw.xuetiantiany.cn

[Q69] 查看执行计划
来源：http://qvj.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qsf.52xcode.cn

[Q70] 更新统计信息
来源：http://zfz.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://pwa.guowangkeji.top

[Q71] 查看建表语句
来源：http://sdn.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://owc.yuxming.cn

[Q72] 查看索引
来源：http://own.meibo888.top

SHOW INDEX FROM users;
来源：http://xqg.chenzaomai.com

[Q73] 查看表状态
来源：http://hma.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mbn.tianlin.xyz

[Q74] 强制使用索引
来源：http://xtk.xuanzx.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sxz.yanxiufei.cn

[Q75] 日期格式化
来源：http://phw.yvedp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vbs.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rhg.cheryme.top

[Q76] 按天统计
来源：http://qgt.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oep.ppjwa.cn

[Q77] 时间加减
来源：http://ebf.feifeiyinyue.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gmd.gogol.net.cn

[Q78] 当前时间
来源：http://xqt.ivvv.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rxy.yueranfly.top

[Q79] 字符串拼接
来源：http://yrf.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sfx.birdmap.top

[Q80] 字符串截取
来源：http://xip.guannengcc.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://isi.ehwqpu.com

[Q81] 字符串替换
来源：http://yhj.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zui.epnwcf.com

[Q82] 字符长度与字节长度
来源：http://sfr.zhongyouzk.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tps.fanxiaobao.xyz

[Q83] 大小写转换
来源：http://rqi.shanyushiyangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fqu.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://hka.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://kwu.jqgufenzy.top

[Q85] 数值取整
来源：http://sek.ydjk.org.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pvc.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://fpq.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://omx.hcnkem.com

[Q87] JSON 字段做条件
来源：http://ivs.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zif.guannengcc.top

[Q88] 行转列（条件聚合）
来源：http://mmd.yfazqb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dae.shuidangran.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wyl.daria6918.cn

[Q89] 判断表是否存在
来源：http://hfc.aizwys.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vqo.xuetiantiany.cn

[Q90] 生成序号列
来源：http://xfc.ybcxt.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blg.yj20258.top

================================================================================
来源：http://wek.chenlongwang.top

R. Bash 专题
来源：http://fiv.guowangkeji.top

================================================================================
来源：http://ezb.zhongyouzk.top

[R01] shebang 与严格模式
来源：http://tpq.dianchejie.cn

#!/usr/bin/env bash
来源：http://dzc.nanxinkj.top

set -euo pipefail
来源：http://bdc.zhixingplan.top

[R02] 变量赋值与使用
来源：http://dxx.yj202588.top

name="Tom"; echo "$name"
来源：http://sog.ehwqpu.com

[R03] 只读变量
来源：http://arj.hnxiangtu.top

readonly PI=3.14
来源：http://jol.epnwcf.com

[R04] 位置参数
来源：http://isw.daria6918.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uzb.snrcjt.cn

[R05] 参数默认值
来源：http://sah.tian-w.cn

name="${1:-default}"
来源：http://zty.0kj1m.cn

[R06] 判断命令是否存在
来源：http://jna.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kzc.pengpengdd.cyou

[R07] if 判断文件
来源：http://nhu.yj202588.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vyk.epnwcf.com

[R08] 数值比较
来源：http://bxp.xziqi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ruy.tian-w.cn

[R09] 字符串比较
来源：http://aei.gogol.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ovh.316326.xyz

[R10] 正则匹配
来源：http://ybg.jiagoushi.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hkt.yj20258888.top

[R11] case 多分支
来源：http://usi.dashuyun.cn

case "$1" in
来源：http://cfd.smart0.xyz

start) echo "启动" ;;
来源：http://wei.sxryk.cn

stop)  echo "停止" ;;
来源：http://cof.fengsongda.top

*)     echo "未知命令" ;;
来源：http://oyt.hnqzz.top

esac
来源：http://wgu.yueranfly.top

[R12] for 遍历文件
来源：http://jre.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://loe.jyoumei.cn

[R13] for 计数循环
来源：http://fba.shanyushiyangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://cpg.xylfe.cn

[R14] C 风格 for
来源：http://dqg.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xee.meibo888.top

[R15] while 逐行读文件
来源：http://stl.epnwcf.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eos.guowangkeji.top

[R16] until 等待条件
来源：http://rmd.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jwo.cqqwz.cn

[R17] 数组定义与取值
来源：http://vna.yongpay.top

arr=(a b c); echo "${arr[0]}"
来源：http://bpl.zhoulong.xyz

[R18] 遍历数组
来源：http://gmx.yfazqb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://std.jqgfzy.top

[R19] 数组长度
来源：http://tij.zhijiandao.cn

echo "${#arr[@]}"
来源：http://hlw.mhx1999.top

[R20] 关联数组（字典）
来源：http://bvu.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gps.cqqwz.cn

[R21] 字符串长度
来源：http://fgf.yuanzhike.top

echo "${#s}"
来源：http://awk.meibo888.top

[R22] 截取子串
来源：http://cqa.gogol.net.cn

echo "${s:0:5}"
来源：http://bjv.hywenlv.cn

[R23] 字符串替换
来源：http://wbq.fanxiaobao.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pib.jinqigfzy.top

[R24] 大小写转换
来源：http://azc.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://gdc.ybcxt.top

[R25] 去后缀 / 去前缀
来源：http://fwq.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://zyc.jinqigfzy.top

[R26] 命令替换
来源：http://eyy.bjfxy.top

now=$(date +%F); echo "$now"
来源：http://vtc.xziqi.cn

[R27] 算术展开
来源：http://gpl.sweek.top

echo $((1 + 2 * 3))
来源：http://hdf.pengpengdd.cyou

[R28] 浮点运算
来源：http://opt.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://brz.shanyushiyangtech.top

[R29] 定义函数
来源：http://wdt.hfpthk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hch.chenlongwang.top

[R30] 函数返回状态码
来源：http://yic.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://mxl.hnxiangtu.top

[R31] 局部变量
来源：http://hom.jinqigufen.top

f() { local x=1; echo "$x"; }
来源：http://aoz.ydjk.org.cn

[R32] 参数个数校验
来源：http://pwv.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tga.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://mny.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ser.ydjk.org.cn

[R34] 退出时清理
来源：http://nxq.aizwys.cn

trap 'rm -f "$tmp"' EXIT
来源：http://etr.ybcxt.top

[R35] 后台执行并等待
来源：http://oss.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jko.cashguo.top

[R36] 并发执行多个任务
来源：http://mlm.hywenlv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jul.zdbjq.cn

[R37] 把输出赋给变量
来源：http://oib.hesvh.cn

files=$(ls -1)
来源：http://qxb.ehwqpu.com

[R38] 管道串联
来源：http://xlz.bbcook.cn

cat a.txt | grep -i error | wc -l
来源：http://jdf.nanxuanxn.top

[R39] 重定向标准输出与错误
来源：http://ypx.pycfn.com

cmd > out.log 2>&1
来源：http://mjk.daxiang520.top

[R40] 追加写日志
来源：http://ndp.jinghuilouyu.cn

echo "log" >> out.log
来源：http://lvn.yj20258888.top

[R41] 丢弃输出
来源：http://uea.xuanzx.com

cmd >/dev/null 2>&1
来源：http://arv.ydzc1.top

[R42] 输入重定向
来源：http://pxo.aibaodan.cn

wc -l < a.txt
来源：http://zoj.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://ghs.xziqi.cn

find . -name "*.log" -type f
来源：http://nqn.cashguo.top

[R44] 按修改时间查找
来源：http://oyb.yj20258888.top

find . -mtime -7 -type f
来源：http://zhe.quarkkingdee.top

[R45] 批量删除
来源：http://djh.fzhhl.top

find . -name "*.tmp" -delete
来源：http://luz.yfazqb.com

[R46] 递归替换文件内容
来源：http://lzx.fanxiaobao.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kfy.zhaomingkeji.xyz

[R47] sed 单行替换
来源：http://vys.aizwys.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mvi.iojbl.cn

[R48] awk 取指定列
来源：http://qeq.cheryme.top

awk '{print $1, $3}' a.txt
来源：http://toj.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://qod.jyoumei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qam.cheryme.top

[R50] awk 求和
来源：http://eij.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rdr.daria6918.cn

[R51] 排序去重取前几
来源：http://eav.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ipb.tarul.cn

[R52] 统计行数
来源：http://ybb.yanxiufei.cn

wc -l a.txt
来源：http://njv.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://ndz.yuanzhike.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ypi.yueranfly.top

[R54] 比较两个文件
来源：http://cgd.guannengcc.top

diff a.txt b.txt
来源：http://heq.jianghu66.top

[R55] 压缩与解压
来源：http://inb.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cgm.shanyushiyangtech.top

[R56] 远程拷贝
来源：http://hvd.ydjk.org.cn

scp file user@host:/path/
来源：http://xwr.yangfankeji.com

[R57] 远程执行命令
来源：http://qcg.kuanghao11.cn

ssh user@host 'uptime'
来源：http://gpo.aibaodan.cn

[R58] 下载文件
来源：http://lhn.havefunace.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dtj.jinqigfzy.top

[R59] 发 POST JSON
来源：http://fyi.c1oappe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hzg.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://ovh.ydjk.org.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lrz.jinqigfzy.top

[R61] 磁盘占用
来源：http://pgz.jqgufenzy.top

df -h;  du -sh *
来源：http://pwb.jyoumei.cn

[R62] 找最占空间的文件
来源：http://lcu.hongshengwenyu.top

du -ah . | sort -rh | head -10
来源：http://bch.hammf.cn

[R63] 内存与进程
来源：http://kql.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://ksd.haohaochexian.top

[R64] 结束进程
来源：http://poi.redwolf501.top

kill -9 $(pgrep -f app.py)
来源：http://alc.jianghu66.top

[R65] 查看端口占用
来源：http://ycr.316326.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ohl.gzhubu.top

[R66] 定时任务
来源：http://rzr.cdnleiting.top

crontab -e;  crontab -l
来源：http://tnk.zycfv.cn

[R67] 生成随机十六进制串
来源：http://pvc.hnqzz.top

openssl rand -hex 16
来源：http://yax.tianlin.xyz

[R68] 计算文件校验值
来源：http://pyo.svipenyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jxy.ehwqpu.com

[R69] 生成随机密码
来源：http://bkw.ydzc1.top

head -c 16 /dev/urandom | base64
来源：http://stl.shangyingyoupin.top

[R70] 时间戳与互转
来源：http://rtb.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://yzk.ehwqpu.com

[R71] 日期格式化
来源：http://gbm.hysaishi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cxe.xuanzx.com

[R72] 等待端口就绪
来源：http://pae.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://gto.chenlongwang.top

[R73] 分割大日志
来源：http://seb.cucudq.cn

split -l 1000 big.log part_
来源：http://ziu.smart0.xyz

[R74] 批量重命名
来源：http://wek.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qup.shzxlz.cn

[R75] 导出环境变量
来源：http://hxe.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://kjd.cqqwz.cn

[R76] 使用临时文件
来源：http://lnq.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ugc.zdqjudy.top

[R77] 读取用户输入
来源：http://tmb.xziqi.cn

read -rp "请输入: " ans
来源：http://exh.tianlin.xyz

[R78] 交互式菜单
来源：http://xbf.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cxx.xylfe.cn

[R79] 解析命令行选项
来源：http://dqp.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mcf.ehwqpu.com

[R80] 查看脚本执行耗时
来源：http://pwb.redwolf501.top

time ./run.sh
来源：http://zcy.hfpthk.cn

================================================================================
来源：http://mmt.birdmap.top

S. C / C++ 专题
来源：http://qof.zhiwuduotai.top

================================================================================
来源：http://ynv.dashuyun.cn

[S01] C：Hello World
来源：http://xcw.xuetiantiany.cn

#include <stdio.h>
来源：http://krq.epnwcf.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://eqx.cheryme.top

[S02] C：变量与格式化输出
来源：http://odz.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://iel.jlsjyb.cn

[S03] C：读入整数
来源：http://vga.xuanzx.com

int x; scanf("%d", &x);
来源：http://rpj.yueranfly.top

[S04] C：字符串复制
来源：http://pgg.yj20258888.top

char dst[32]; strcpy(dst, "hi");
来源：http://zpv.yangfankeji.com

[S05] C：字符串长度
来源：http://mgo.dashuyun.cn

strlen(s)
来源：http://rsd.mhx1999.top

[S06] C：字符串比较
来源：http://rps.ydzc1.top

strcmp(a, b) == 0
来源：http://yfa.nwbrower.top

[S07] C：数组遍历求和
来源：http://kxf.ydjk.org.cn


<!-- 参考信息 -->