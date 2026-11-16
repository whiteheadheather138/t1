代发 wailian999

[Q44] IN 子查询
来源：http://kmu.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lbz.shanyushiyangtech.top

[Q45] EXISTS 判断存在
来源：http://kny.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xpr.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://lfj.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zuc.xuanzx.com

[Q47] 与平均值比较
来源：http://mdw.shzxlz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ags.feifeiyinyue.top

[Q48] CTE 公用表表达式
来源：http://ycx.ywan-chungtsiang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uhx.bbcook.cn

SELECT * FROM t WHERE c > 5;
来源：http://dow.ctjpmb.com

[Q49] 更新单行
来源：http://hcb.0kj1m.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ozf.zycfv.cn

[Q50] 批量更新
来源：http://oej.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wkk.chenzaomai.com

[Q51] 用子查询更新
来源：http://iis.hnxiangtu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rzm.andypj.xyz

[Q52] 删除指定行
来源：http://yky.smart0.xyz

DELETE FROM users WHERE id = 10;
来源：http://fut.dashuyun.cn

[Q53] 按条件删除
来源：http://ahu.ppjwa.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gze.iojbl.cn

[Q54] 清空表
来源：http://ubp.sxryk.cn

TRUNCATE TABLE logs;
来源：http://swz.c1oappe.top

[Q55] 排名（并列占位）
来源：http://skd.hysaishi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://liz.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://gfm.svipenyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lpg.yvedp.cn

[Q57] 行号
来源：http://rsx.shuidangran.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fjg.iojbl.cn

[Q58] 累计求和
来源：http://fpq.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bfn.wangshuangyany.cn

[Q59] 分组内累计
来源：http://xsj.haohaochexian.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dnk.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://bgl.iojbl.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ucb.wangdashe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ocd.svipenyu.cn

[Q61] 移动平均
来源：http://xkv.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fxp.yvedp.cn

[Q62] 分组占比
来源：http://gin.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pin.ivvv.top

[Q63] 开启事务
来源：http://udf.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rxw.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://xpa.9152youxi.cn

COMMIT;
来源：http://rqe.c1oappe.top

[Q65] 回滚事务
来源：http://rjf.xylfe.cn

ROLLBACK;
来源：http://udk.daria6918.cn

[Q66] 行锁查询
来源：http://mqy.jinyuanbaomall.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mcb.sysykeji.top

[Q67] 设置隔离级别
来源：http://wgk.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jaa.hesvh.cn

[Q68] 保存点
来源：http://cwn.fanxiaobao.xyz

SAVEPOINT sp1;
来源：http://wqv.hesvh.cn

ROLLBACK TO sp1;
来源：http://lnf.xingfuxueyuan.xyz

[Q69] 查看执行计划
来源：http://xtd.feifeiyinyue.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gpp.bbcook.cn

[Q70] 更新统计信息
来源：http://tty.hfpthk.cn

ANALYZE TABLE users;
来源：http://pbt.jinqigufen.top

[Q71] 查看建表语句
来源：http://lio.jinyuanbaomall.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://txu.nanxinkj.top

[Q72] 查看索引
来源：http://ypj.0kj1m.cn

SHOW INDEX FROM users;
来源：http://hae.xziqi.cn

[Q73] 查看表状态
来源：http://axz.vqdsnc.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kwn.gogol.net.cn

[Q74] 强制使用索引
来源：http://ose.tarul.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qhe.shangyingyoupin.top

[Q75] 日期格式化
来源：http://zby.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oye.dashuyun.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hth.hesvh.cn

[Q76] 按天统计
来源：http://uan.vqdsnc.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wvc.birdmap.top

[Q77] 时间加减
来源：http://mwj.c1oappe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jph.gogol.net.cn

[Q78] 当前时间
来源：http://qju.gzhubu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aac.hnqzz.top

[Q79] 字符串拼接
来源：http://hvt.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://flo.hesvh.cn

[Q80] 字符串截取
来源：http://gti.jianghu66.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://awf.mhx1999.top

[Q81] 字符串替换
来源：http://fhu.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://any.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://hso.ybcxt.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cja.zdbjq.cn

[Q83] 大小写转换
来源：http://qcr.yj20258.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bxv.mhx1999.top

[Q84] 去除首尾空格
来源：http://dnc.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://hha.chenjidiqi.icu

[Q85] 数值取整
来源：http://lov.sjlbkw.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yvh.yj202588.top

[Q86] 读取 JSON 字段
来源：http://nbz.jinyuanbaomall.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://juc.yj20258.top

[Q87] JSON 字段做条件
来源：http://odp.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yts.jlsjyb.cn

[Q88] 行转列（条件聚合）
来源：http://qmg.nanxuanxn.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://unb.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gas.shzxlz.cn

[Q89] 判断表是否存在
来源：http://ocn.xingfuxueyuan.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zep.vehdjk.com

[Q90] 生成序号列
来源：http://cbv.sxryk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dxa.shzxlz.cn

================================================================================
来源：http://rvf.jlsjyb.cn

R. Bash 专题
来源：http://tta.nwbrower.top

================================================================================
来源：http://vnn.316326.xyz

[R01] shebang 与严格模式
来源：http://xpj.aizwys.cn

#!/usr/bin/env bash
来源：http://yav.epnwcf.com

set -euo pipefail
来源：http://cmx.yvedp.cn

[R02] 变量赋值与使用
来源：http://rgi.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://ccr.fktsv.cn

[R03] 只读变量
来源：http://zmv.fehbvm.com

readonly PI=3.14
来源：http://lkw.shangyingyoupin.top

[R04] 位置参数
来源：http://yxh.ivvv.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mon.tarul.cn

[R05] 参数默认值
来源：http://nzv.gogol.net.cn

name="${1:-default}"
来源：http://mpx.wangdashe.top

[R06] 判断命令是否存在
来源：http://ytq.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gzi.ctjpmb.com

[R07] if 判断文件
来源：http://oaf.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dpd.yuxming.cn

[R08] 数值比较
来源：http://ywc.sysykeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://imr.hnqzz.top

[R09] 字符串比较
来源：http://ofw.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gjd.hnqzz.top

[R10] 正则匹配
来源：http://cml.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://phs.fzhhl.top

[R11] case 多分支
来源：http://fku.jinyuanbaomall.cn

case "$1" in
来源：http://wnc.jlsjyb.cn

start) echo "启动" ;;
来源：http://sih.bbcook.cn

stop)  echo "停止" ;;
来源：http://usf.zycfv.cn

*)     echo "未知命令" ;;
来源：http://gnf.yonumen.top

esac
来源：http://hmj.hywenlv.cn

[R12] for 遍历文件
来源：http://dqt.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://wti.tanke756.top

[R13] for 计数循环
来源：http://cjp.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://ktp.jinghuilouyu.cn

[R14] C 风格 for
来源：http://wve.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://txb.shanyushiyangtech.top

[R15] while 逐行读文件
来源：http://abs.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jay.daria6918.cn

[R16] until 等待条件
来源：http://vsz.9152youxi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yoq.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://lug.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://rjw.tian-w.cn

[R18] 遍历数组
来源：http://zuv.pycfn.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://elb.tianlin.xyz

[R19] 数组长度
来源：http://bml.shangyingyoupin.top

echo "${#arr[@]}"
来源：http://zti.smart0.xyz

[R20] 关联数组（字典）
来源：http://gmn.dashuyun.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jlr.shanyushiyangkeji.top

[R21] 字符串长度
来源：http://bho.gotoacloud.top

echo "${#s}"
来源：http://can.hcnkem.com

[R22] 截取子串
来源：http://wnt.zdqjudy.top

echo "${s:0:5}"
来源：http://evt.shzxlz.cn

[R23] 字符串替换
来源：http://yox.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ovk.haohaochexian.top

[R24] 大小写转换
来源：http://nco.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://vcx.yj202588.top

[R25] 去后缀 / 去前缀
来源：http://dfx.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://cdn.gotoacloud.top

[R26] 命令替换
来源：http://dqs.quarkkingdee.top

now=$(date +%F); echo "$now"
来源：http://cqz.zycfv.cn

[R27] 算术展开
来源：http://pje.kuanghao11.cn

echo $((1 + 2 * 3))
来源：http://lug.nwbrower.top

[R28] 浮点运算
来源：http://sld.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://ces.fehbvm.com

[R29] 定义函数
来源：http://ibb.vehdjk.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zyb.zhongyouzk.top

[R30] 函数返回状态码
来源：http://mru.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://vyw.xylfe.cn

[R31] 局部变量
来源：http://cqe.hammf.cn

f() { local x=1; echo "$x"; }
来源：http://zhe.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://rft.jlsjyb.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dih.nwbrower.top

[R33] 捕获错误并提示行号
来源：http://que.jinqigfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ezp.zhiwuduotai.top

[R34] 退出时清理
来源：http://ase.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kzv.xylfe.cn

[R35] 后台执行并等待
来源：http://hkr.redwolf501.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vpz.shzxlz.cn

[R36] 并发执行多个任务
来源：http://uzq.hongshengwenyu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://imj.c1oappe.top

[R37] 把输出赋给变量
来源：http://rcv.hfpthk.cn

files=$(ls -1)
来源：http://efk.yfazqb.com

[R38] 管道串联
来源：http://fxw.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://uxk.jinqigfzy.top

[R39] 重定向标准输出与错误
来源：http://qnd.xingfuxueyuan.xyz

cmd > out.log 2>&1
来源：http://mkg.jqgufenzy.top

[R40] 追加写日志
来源：http://eja.zhengqikj.top

echo "log" >> out.log
来源：http://ohz.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://tkd.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://nmd.ivvv.top

[R42] 输入重定向
来源：http://csu.redwolf501.top

wc -l < a.txt
来源：http://ibr.yj202588.top

[R43] 按名字查找文件
来源：http://tyt.hnxiangtu.top

find . -name "*.log" -type f
来源：http://iqe.svipenyu.cn

[R44] 按修改时间查找
来源：http://kka.sxryk.cn

find . -mtime -7 -type f
来源：http://kgl.yj20258888.top

[R45] 批量删除
来源：http://euv.shuidangran.top

find . -name "*.tmp" -delete
来源：http://ppx.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://qmm.gaohongyu789.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qwk.vehdjk.com

[R47] sed 单行替换
来源：http://cbh.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://lyb.c1oappe.top

[R48] awk 取指定列
来源：http://csi.sxryk.cn

awk '{print $1, $3}' a.txt
来源：http://uyn.c1oappe.top

[R49] awk 带条件
来源：http://ync.chenlongwang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iae.sjlbkw.cn

[R50] awk 求和
来源：http://jwq.gaohongyu789.top

awk '{s += $2} END {print s}' a.txt
来源：http://tcl.guannengcc.top

[R51] 排序去重取前几
来源：http://txx.tian-w.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fum.zycfv.cn

[R52] 统计行数
来源：http://off.xuanzx.com

wc -l a.txt
来源：http://dqt.hongshengwenyu.top

[R53] 查看文件头与实时尾
来源：http://ikb.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yeg.zhoulong.xyz

[R54] 比较两个文件
来源：http://pwg.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://iao.hongshengwenyu.top

[R55] 压缩与解压
来源：http://spz.zdqjudy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sxa.9152youxi.cn

[R56] 远程拷贝
来源：http://sxa.chenlongwang.top

scp file user@host:/path/
来源：http://qss.chenjidiqi.icu

[R57] 远程执行命令
来源：http://dit.xuanzx.com

ssh user@host 'uptime'
来源：http://rql.yangfankeji.com

[R58] 下载文件
来源：http://str.guowangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gja.shzxlz.cn

[R59] 发 POST JSON
来源：http://pjc.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rrz.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://lxm.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uvt.yj20258.top

[R61] 磁盘占用
来源：http://reh.sysykeji.top

df -h;  du -sh *
来源：http://bom.birdmap.top

[R62] 找最占空间的文件
来源：http://lmg.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://sne.ehwqpu.com

[R63] 内存与进程
来源：http://jpy.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://qbr.nanxuanxn.top

[R64] 结束进程
来源：http://hhw.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://rqh.snrcjt.cn

[R65] 查看端口占用
来源：http://mlb.guannengcc.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gou.xuanzx.com

[R66] 定时任务
来源：http://xxa.chenjidiqi.icu

crontab -e;  crontab -l
来源：http://wvp.yanxiufei.cn

[R67] 生成随机十六进制串
来源：http://zne.yuanzhike.top

openssl rand -hex 16
来源：http://oan.jianghu66.top

[R68] 计算文件校验值
来源：http://dfo.cheryme.top

sha256sum a.txt;  md5sum a.txt
来源：http://bys.nanxinkj.top

[R69] 生成随机密码
来源：http://hrn.sweek.top

head -c 16 /dev/urandom | base64
来源：http://kem.xziqi.cn

[R70] 时间戳与互转
来源：http://kbk.xuetiantiany.cn

date +%s;  date -d @1700000000
来源：http://kfn.ctjpmb.com

[R71] 日期格式化
来源：http://qld.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://uvz.guowangkeji.top

[R72] 等待端口就绪
来源：http://siv.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dgh.gaohongyu789.top

[R73] 分割大日志
来源：http://rob.sjlbkw.cn

split -l 1000 big.log part_
来源：http://oqi.vehdjk.com

[R74] 批量重命名
来源：http://fyi.zhaomingkeji.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wgo.316326.xyz

[R75] 导出环境变量
来源：http://rav.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://fmz.tian-w.cn

[R76] 使用临时文件
来源：http://uni.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uak.ydzc1.top

[R77] 读取用户输入
来源：http://sbu.wangdashe.top

read -rp "请输入: " ans
来源：http://pen.tanke756.top

[R78] 交互式菜单
来源：http://qde.zhongyouzk.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nhh.ppjwa.cn

[R79] 解析命令行选项
来源：http://nkh.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ykv.yuxming.cn

[R80] 查看脚本执行耗时
来源：http://tjx.fktsv.cn

time ./run.sh
来源：http://yng.shuidangran.top

================================================================================
来源：http://jwf.gogol.net.cn

S. C / C++ 专题
来源：http://gkw.yongpay.top

================================================================================
来源：http://ipw.zhengqikj.top

[S01] C：Hello World
来源：http://uvf.meibo888.top

#include <stdio.h>
来源：http://pww.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://abq.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://tjl.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://xns.hammf.cn

[S03] C：读入整数
来源：http://xpt.ehwqpu.com

int x; scanf("%d", &x);
来源：http://zbw.hnxiangtu.top

[S04] C：字符串复制
来源：http://dgo.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vpj.xylfe.cn

[S05] C：字符串长度
来源：http://zlo.xuanzx.com

strlen(s)
来源：http://lnl.gogol.net.cn

[S06] C：字符串比较
来源：http://zhu.yuanzhike.top

strcmp(a, b) == 0
来源：http://vya.shuidangran.top

[S07] C：数组遍历求和
来源：http://faa.hcnkem.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kxy.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://phk.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tnf.meibo888.top

[S09] C：结构体定义与初始化
来源：http://ytu.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dfh.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://svg.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://gtz.pycfn.com

[S11] C：逐行读文件
来源：http://hzj.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://rzl.havefunace.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://exg.zycfv.cn

fclose(f);
来源：http://dth.zhengqikj.top

[S12] C：写文件
来源：http://fya.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qow.yj202588.top

[S13] C：宏定义
来源：http://lag.tianlin.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kio.meibo888.top

[S14] C：枚举
来源：http://cyb.bbcook.cn


<!-- 参考信息 -->