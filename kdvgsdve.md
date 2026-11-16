代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://aig.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://qev.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://fao.hongshengwenyu.top

[Q42] 连接条件附加过滤
来源：http://hga.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://ojg.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hwj.havefunace.top

[Q43] 标量子查询
来源：http://ixc.dianchejie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tai.yj202588.top

[Q44] IN 子查询
来源：http://xlr.redwolf501.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://viw.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://pju.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://csm.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://qlc.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kgm.tianlin.xyz

[Q47] 与平均值比较
来源：http://lsy.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rta.bjfxy.top

[Q48] CTE 公用表表达式
来源：http://luo.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cwl.chenzaomai.com

SELECT * FROM t WHERE c > 5;
来源：http://jgk.ydjk.org.cn

[Q49] 更新单行
来源：http://axy.gaohongyu789.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jco.sjlbkw.cn

[Q50] 批量更新
来源：http://lrd.gogol.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gwu.hnqzz.top

[Q51] 用子查询更新
来源：http://xcj.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ycd.hnxiangtu.top

[Q52] 删除指定行
来源：http://xyu.jianghu66.top

DELETE FROM users WHERE id = 10;
来源：http://ppv.tanke756.top

[Q53] 按条件删除
来源：http://pno.zhongyouzk.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rrd.sufxvd.cn

[Q54] 清空表
来源：http://rbn.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://zgh.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://kwo.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qjd.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://eos.wangshuangyany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bxe.jqgufenzy.top

[Q57] 行号
来源：http://tvy.quarkkingdee.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mjk.jinqigufen.top

[Q58] 累计求和
来源：http://hpx.xuanzx.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uht.0kj1m.cn

[Q59] 分组内累计
来源：http://qdj.guannengcc.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pkf.haohaochexian.top

[Q60] 取上一行 / 下一行
来源：http://rsk.yfazqb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pij.vehdjk.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kaj.ppjwa.cn

[Q61] 移动平均
来源：http://ihx.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://npq.yj202588.top

[Q62] 分组占比
来源：http://dok.sufxvd.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pkz.yongpay.top

[Q63] 开启事务
来源：http://clh.jinqigfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fcw.redwolf501.top

[Q64] 提交事务
来源：http://rse.cheryme.top

COMMIT;
来源：http://cmj.zycfv.cn

[Q65] 回滚事务
来源：http://puu.bjfxy.top

ROLLBACK;
来源：http://pob.sjlbkw.cn

[Q66] 行锁查询
来源：http://zlc.guowangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cgj.chenjidiqi.icu

[Q67] 设置隔离级别
来源：http://vqa.yj202588.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pkh.ydjk.org.cn

[Q68] 保存点
来源：http://hcs.feifeiyinyue.top

SAVEPOINT sp1;
来源：http://qix.wangdashe.top

ROLLBACK TO sp1;
来源：http://fsl.zhiwuduotai.top

[Q69] 查看执行计划
来源：http://wos.snrcjt.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://txc.ehwqpu.com

[Q70] 更新统计信息
来源：http://mqw.fktsv.cn

ANALYZE TABLE users;
来源：http://opx.cucudq.cn

[Q71] 查看建表语句
来源：http://qdi.yfazqb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hck.ctjpmb.com

[Q72] 查看索引
来源：http://spy.yangfankeji.com

SHOW INDEX FROM users;
来源：http://aij.cheryme.top

[Q73] 查看表状态
来源：http://oeo.hywenlv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oyv.ydjk.org.cn

[Q74] 强制使用索引
来源：http://dli.zhixingplan.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lwy.chenzaomai.com

[Q75] 日期格式化
来源：http://qmp.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ngx.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ahf.pycfn.com

[Q76] 按天统计
来源：http://zxp.jinqigufen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cnv.birdmap.top

[Q77] 时间加减
来源：http://sdq.9152youxi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://saq.52xcode.cn

[Q78] 当前时间
来源：http://cpl.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fzu.ywan-chungtsiang.top

[Q79] 字符串拼接
来源：http://aqh.wangshuangyany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://knq.yueranfly.top

[Q80] 字符串截取
来源：http://kxp.wangshuangyany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vkk.yuxming.cn

[Q81] 字符串替换
来源：http://dhv.ydzc1.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bsj.xylfe.cn

[Q82] 字符长度与字节长度
来源：http://cji.yanxiufei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dmb.cdnleiting.top

[Q83] 大小写转换
来源：http://pdb.bjfxy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ral.uphjek.com

[Q84] 去除首尾空格
来源：http://upr.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://esi.vqdsnc.cn

[Q85] 数值取整
来源：http://bbz.tarul.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bbr.wangshuangyany.cn

[Q86] 读取 JSON 字段
来源：http://zxk.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ymt.smart0.xyz

[Q87] JSON 字段做条件
来源：http://ezv.wangshuangyany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://onm.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://qvi.316326.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://inz.meibo888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rkt.gogol.net.cn

[Q89] 判断表是否存在
来源：http://fcn.redwolf501.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://unv.tarul.cn

[Q90] 生成序号列
来源：http://ywh.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pdb.cashguo.top

================================================================================
来源：http://rqv.sjlbkw.cn

R. Bash 专题
来源：http://jtg.redwolf501.top

================================================================================
来源：http://ody.pycfn.com

[R01] shebang 与严格模式
来源：http://bnl.cqqwz.cn

#!/usr/bin/env bash
来源：http://uxr.yj20258888.top

set -euo pipefail
来源：http://swz.wangshuangyany.cn

[R02] 变量赋值与使用
来源：http://zwp.svipenyu.cn

name="Tom"; echo "$name"
来源：http://uaq.svipenyu.cn

[R03] 只读变量
来源：http://dcu.yfazqb.com

readonly PI=3.14
来源：http://kwn.hysaishi.cn

[R04] 位置参数
来源：http://vqs.tarul.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oxo.vehdjk.com

[R05] 参数默认值
来源：http://vja.yvedp.cn

name="${1:-default}"
来源：http://omc.birdmap.top

[R06] 判断命令是否存在
来源：http://grb.cashguo.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://peb.ivvv.top

[R07] if 判断文件
来源：http://evt.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qnb.0kj1m.cn

[R08] 数值比较
来源：http://nbo.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sbs.hnqzz.top

[R09] 字符串比较
来源：http://nar.yonumen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wqj.birdmap.top

[R10] 正则匹配
来源：http://sdt.fzhhl.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://adn.ctjpmb.com

[R11] case 多分支
来源：http://uvi.dashuyun.cn

case "$1" in
来源：http://zwd.jqgfzy.top

start) echo "启动" ;;
来源：http://kbq.daxiang520.top

stop)  echo "停止" ;;
来源：http://dtx.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://vex.gotoacloud.top

esac
来源：http://zoa.cucudq.cn

[R12] for 遍历文件
来源：http://oud.jqgfzy.top

for f in *.txt; do echo "$f"; done
来源：http://cdx.daria6918.cn

[R13] for 计数循环
来源：http://yeq.guowangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://rrk.yonumen.top

[R14] C 风格 for
来源：http://odw.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bly.ivvv.top

[R15] while 逐行读文件
来源：http://rjl.sysykeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://leh.tarul.cn

[R16] until 等待条件
来源：http://pug.ehwqpu.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rhu.ivvv.top

[R17] 数组定义与取值
来源：http://hkb.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oox.nwbrower.top

[R18] 遍历数组
来源：http://qtg.cucudq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xwl.meibo888.top

[R19] 数组长度
来源：http://cgy.9152youxi.cn

echo "${#arr[@]}"
来源：http://ixm.fzhhl.top

[R20] 关联数组（字典）
来源：http://bxy.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://euy.jlsjyb.cn

[R21] 字符串长度
来源：http://uuv.chenlongwang.top

echo "${#s}"
来源：http://fzn.yongpay.top

[R22] 截取子串
来源：http://ing.zdqjudy.top

echo "${s:0:5}"
来源：http://zdn.guowangkeji.top

[R23] 字符串替换
来源：http://lfb.sysykeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sxc.hnxiangtu.top

[R24] 大小写转换
来源：http://xhp.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://yde.nanxuanxn.top

[R25] 去后缀 / 去前缀
来源：http://vmm.wangdashe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hry.bjfxy.top

[R26] 命令替换
来源：http://lkb.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://fva.hnxiangtu.top

[R27] 算术展开
来源：http://cna.iojbl.cn

echo $((1 + 2 * 3))
来源：http://ebz.c1oappe.top

[R28] 浮点运算
来源：http://pye.cdnleiting.top

echo "scale=2; 10/3" | bc
来源：http://jis.fanxiaobao.xyz

[R29] 定义函数
来源：http://gja.svipenyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xgh.aibaodan.cn

[R30] 函数返回状态码
来源：http://vhh.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://hbc.dashuyun.cn

[R31] 局部变量
来源：http://eef.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://zeo.cheryme.top

[R32] 参数个数校验
来源：http://usg.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://evj.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://hmv.daria6918.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qsl.gzhubu.top

[R34] 退出时清理
来源：http://fbs.smart0.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://qaw.jyoumei.cn

[R35] 后台执行并等待
来源：http://loa.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hao.smart0.xyz

[R36] 并发执行多个任务
来源：http://hqg.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jqr.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://dcr.gzhubu.top

files=$(ls -1)
来源：http://glp.quarkkingdee.top

[R38] 管道串联
来源：http://lzp.jiagoushi.top

cat a.txt | grep -i error | wc -l
来源：http://lye.0kj1m.cn

[R39] 重定向标准输出与错误
来源：http://pbl.gaohongyu789.top

cmd > out.log 2>&1
来源：http://uew.xinyue.icu

[R40] 追加写日志
来源：http://wax.zhoulong.xyz

echo "log" >> out.log
来源：http://yxf.shzxlz.cn

[R41] 丢弃输出
来源：http://urj.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://ptd.jyoumei.cn

[R42] 输入重定向
来源：http://wap.smart0.xyz

wc -l < a.txt
来源：http://rpq.andypj.xyz

[R43] 按名字查找文件
来源：http://ajv.yongpay.top

find . -name "*.log" -type f
来源：http://ofr.52xcode.cn

[R44] 按修改时间查找
来源：http://psv.xziqi.cn

find . -mtime -7 -type f
来源：http://nos.iojbl.cn

[R45] 批量删除
来源：http://wne.jiagoushi.top

find . -name "*.tmp" -delete
来源：http://uqe.havefunace.top

[R46] 递归替换文件内容
来源：http://cou.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://icy.xziqi.cn

[R47] sed 单行替换
来源：http://ycv.svipenyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nyb.hysaishi.cn

[R48] awk 取指定列
来源：http://ukm.sufxvd.cn

awk '{print $1, $3}' a.txt
来源：http://sgl.c1oappe.top

[R49] awk 带条件
来源：http://qgk.zhaomingkeji.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ngd.haohaochexian.top

[R50] awk 求和
来源：http://rdd.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://blu.tanke756.top

[R51] 排序去重取前几
来源：http://his.jiagoushi.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ptb.zdbjq.cn

[R52] 统计行数
来源：http://rpy.sweek.top

wc -l a.txt
来源：http://vih.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://cpx.hongshengwenyu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cjb.feifeiyinyue.top

[R54] 比较两个文件
来源：http://eny.tianlin.xyz

diff a.txt b.txt
来源：http://zdp.ppjwa.cn

[R55] 压缩与解压
来源：http://vgj.zhengqikj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lpf.sxryk.cn

[R56] 远程拷贝
来源：http://bxd.52xcode.cn

scp file user@host:/path/
来源：http://mbv.daxiang520.top

[R57] 远程执行命令
来源：http://zud.jinqigfzy.top

ssh user@host 'uptime'
来源：http://sxm.sysykeji.top

[R58] 下载文件
来源：http://fgx.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uwz.gotoacloud.top

[R59] 发 POST JSON
来源：http://hvs.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://llu.iojbl.cn

[R60] 只看 HTTP 状态码
来源：http://ngk.shangyingyoupin.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fft.zhoulong.xyz

[R61] 磁盘占用
来源：http://wcp.9152youxi.cn

df -h;  du -sh *
来源：http://vpt.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://xwl.cashguo.top

du -ah . | sort -rh | head -10
来源：http://skv.redwolf501.top

[R63] 内存与进程
来源：http://iuz.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://wqg.yangfankeji.com

[R64] 结束进程
来源：http://mer.andypj.xyz

kill -9 $(pgrep -f app.py)
来源：http://otw.redwolf501.top

[R65] 查看端口占用
来源：http://cct.zhixingplan.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eij.xuetiantiany.cn

[R66] 定时任务
来源：http://hci.daria6918.cn

crontab -e;  crontab -l
来源：http://hux.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://khl.xuetiantiany.cn

openssl rand -hex 16
来源：http://eoz.uphjek.com

[R68] 计算文件校验值
来源：http://lrn.yj20258888.top

sha256sum a.txt;  md5sum a.txt
来源：http://ktk.shanyushiyangkeji.top

[R69] 生成随机密码
来源：http://zhx.9152youxi.cn

head -c 16 /dev/urandom | base64
来源：http://eeo.xuanzx.com

[R70] 时间戳与互转
来源：http://wpu.sweek.top

date +%s;  date -d @1700000000
来源：http://nkr.cheryme.top

[R71] 日期格式化
来源：http://fkn.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://eko.jqgufenzy.top

[R72] 等待端口就绪
来源：http://ouv.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qux.smart0.xyz

[R73] 分割大日志
来源：http://dic.hywenlv.cn

split -l 1000 big.log part_
来源：http://ndc.xingfuxueyuan.xyz

[R74] 批量重命名
来源：http://xwt.cashguo.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://clt.vqdsnc.cn

[R75] 导出环境变量
来源：http://zuz.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://ato.guowangkeji.top

[R76] 使用临时文件
来源：http://llv.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mxm.ppjwa.cn

[R77] 读取用户输入
来源：http://kqb.yanxiufei.cn

read -rp "请输入: " ans
来源：http://kfr.fanxiaobao.xyz

[R78] 交互式菜单
来源：http://ipv.feifeiyinyue.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wnc.yj20258888.top

[R79] 解析命令行选项
来源：http://hzq.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://edw.shanyushiyangkeji.top

[R80] 查看脚本执行耗时
来源：http://qos.yuxming.cn

time ./run.sh
来源：http://nft.wangshuangyany.cn

================================================================================
来源：http://slh.yj202588.top

S. C / C++ 专题
来源：http://erj.yangfankeji.com

================================================================================
来源：http://wzt.hywenlv.cn

[S01] C：Hello World
来源：http://hze.cucudq.cn

#include <stdio.h>
来源：http://jhc.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hvs.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://sam.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://lcw.feifeiyinyue.top

[S03] C：读入整数
来源：http://phe.zhixingplan.top

int x; scanf("%d", &x);
来源：http://inl.hesvh.cn

[S04] C：字符串复制
来源：http://luo.jianghu66.top

char dst[32]; strcpy(dst, "hi");
来源：http://tpu.daria6918.cn

[S05] C：字符串长度
来源：http://lzd.fengsongda.top

strlen(s)
来源：http://zsi.guowangkeji.top

[S06] C：字符串比较
来源：http://gic.yj202588.top

strcmp(a, b) == 0
来源：http://hpu.yj20258888.top

[S07] C：数组遍历求和
来源：http://wsc.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oyr.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://phv.bjfxy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gwo.zycfv.cn

[S09] C：结构体定义与初始化
来源：http://joh.jqgfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nkd.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://tjs.yfazqb.com

int *p = &a;  *p = 5;
来源：http://imr.ywan-chungtsiang.top

[S11] C：逐行读文件
来源：http://wnz.wangdashe.top


<!-- 参考信息 -->