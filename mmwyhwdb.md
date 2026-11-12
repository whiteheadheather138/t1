代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://fxr.yuanzhike.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ldt.ctjpmb.com

[Q47] 与平均值比较
来源：http://wvp.guannengcc.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qlb.yj20258.top

[Q48] CTE 公用表表达式
来源：http://okt.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xye.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://wax.daria6918.cn

[Q49] 更新单行
来源：http://yoj.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ajf.dianchejie.cn

[Q50] 批量更新
来源：http://ful.kuanghao11.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ruv.sysykeji.top

[Q51] 用子查询更新
来源：http://xow.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jkl.redwolf501.top

[Q52] 删除指定行
来源：http://uka.wangshuangyany.cn

DELETE FROM users WHERE id = 10;
来源：http://jcl.zycfv.cn

[Q53] 按条件删除
来源：http://ymx.jlsjyb.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://twr.pengpengdd.cyou

[Q54] 清空表
来源：http://brm.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://jfi.yueranfly.top

[Q55] 排名（并列占位）
来源：http://iqy.pycfn.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zwb.svipenyu.cn

[Q56] 密集排名（并列不占位）
来源：http://xuy.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nrf.yuanzhike.top

[Q57] 行号
来源：http://dnd.jianghu66.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fso.52xcode.cn

[Q58] 累计求和
来源：http://ctv.zhiwuduotai.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qvk.cheryme.top

[Q59] 分组内累计
来源：http://dfw.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vwk.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://cro.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uzj.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mht.chenjidiqi.icu

[Q61] 移动平均
来源：http://oaf.gaohongyu789.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://usn.ydjk.org.cn

[Q62] 分组占比
来源：http://jjb.guowangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://goi.sweek.top

[Q63] 开启事务
来源：http://ofi.cdnleiting.top

START TRANSACTION;                -- 或 BEGIN
来源：http://juz.jqgfzy.top

[Q64] 提交事务
来源：http://yts.nanxinkj.top

COMMIT;
来源：http://bht.pycfn.com

[Q65] 回滚事务
来源：http://fbf.sufxvd.cn

ROLLBACK;
来源：http://dqd.gzhubu.top

[Q66] 行锁查询
来源：http://ppg.sxryk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wlt.redwolf501.top

[Q67] 设置隔离级别
来源：http://myd.sufxvd.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pup.yanxiufei.cn

[Q68] 保存点
来源：http://gmz.wangdashe.top

SAVEPOINT sp1;
来源：http://hoi.ehwqpu.com

ROLLBACK TO sp1;
来源：http://xxm.nwbrower.top

[Q69] 查看执行计划
来源：http://yem.jianghu66.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tmy.guannengcc.top

[Q70] 更新统计信息
来源：http://evu.bbcook.cn

ANALYZE TABLE users;
来源：http://saz.guowangkeji.top

[Q71] 查看建表语句
来源：http://lul.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://avh.nanxuanxn.top

[Q72] 查看索引
来源：http://vpb.9152youxi.cn

SHOW INDEX FROM users;
来源：http://mcj.hnqzz.top

[Q73] 查看表状态
来源：http://fap.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tzf.cqqwz.cn

[Q74] 强制使用索引
来源：http://qvr.epnwcf.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ylm.sjlbkw.cn

[Q75] 日期格式化
来源：http://otz.zhiwuduotai.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mtv.bbcook.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vmv.hfpthk.cn

[Q76] 按天统计
来源：http://jyj.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://que.yvedp.cn

[Q77] 时间加减
来源：http://emt.cdnleiting.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vwq.cheryme.top

[Q78] 当前时间
来源：http://shn.hongshengwenyu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zgz.hfpthk.cn

[Q79] 字符串拼接
来源：http://txf.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zsn.yongpay.top

[Q80] 字符串截取
来源：http://jtl.smart0.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zrr.vqdsnc.cn

[Q81] 字符串替换
来源：http://qzp.ydjk.org.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tgu.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://vhc.jlsjyb.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://poq.yuxming.cn

[Q83] 大小写转换
来源：http://ccv.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fsh.chenlongwang.top

[Q84] 去除首尾空格
来源：http://kwg.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://jdm.yanxiufei.cn

[Q85] 数值取整
来源：http://dfs.iojbl.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tci.hammf.cn

[Q86] 读取 JSON 字段
来源：http://uzd.sufxvd.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ubq.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://jbf.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hor.shzxlz.cn

[Q88] 行转列（条件聚合）
来源：http://mwb.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kzz.gogol.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qpk.ehwqpu.com

[Q89] 判断表是否存在
来源：http://dkg.yuxming.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eog.epnwcf.com

[Q90] 生成序号列
来源：http://xdr.uphjek.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xjm.yj20258888.top

================================================================================
来源：http://tka.haohaochexian.top

R. Bash 专题
来源：http://rrt.0kj1m.cn

================================================================================
来源：http://ons.hcnkem.com

[R01] shebang 与严格模式
来源：http://zgw.gogol.net.cn

#!/usr/bin/env bash
来源：http://fag.ywan-chungtsiang.top

set -euo pipefail
来源：http://ugl.aibaodan.cn

[R02] 变量赋值与使用
来源：http://lmz.birdmap.top

name="Tom"; echo "$name"
来源：http://hbk.zhiwuduotai.top

[R03] 只读变量
来源：http://app.316326.xyz

readonly PI=3.14
来源：http://cbr.cashguo.top

[R04] 位置参数
来源：http://cos.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://myp.vehdjk.com

[R05] 参数默认值
来源：http://nqa.hnxiangtu.top

name="${1:-default}"
来源：http://utz.kuanghao11.cn

[R06] 判断命令是否存在
来源：http://sbg.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://utl.jinqigufen.top

[R07] if 判断文件
来源：http://uxk.daria6918.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wkd.hesvh.cn

[R08] 数值比较
来源：http://srr.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dsn.nanxinkj.top

[R09] 字符串比较
来源：http://qqw.hnqzz.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fpb.iojbl.cn

[R10] 正则匹配
来源：http://nxi.guannengcc.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uuu.zhijiandao.cn

[R11] case 多分支
来源：http://ivo.gogol.net.cn

case "$1" in
来源：http://qhd.xuetiantiany.cn

start) echo "启动" ;;
来源：http://cik.havefunace.top

stop)  echo "停止" ;;
来源：http://ejb.vqdsnc.cn

*)     echo "未知命令" ;;
来源：http://qcc.tarul.cn

esac
来源：http://jfi.yanxiufei.cn

[R12] for 遍历文件
来源：http://qkk.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://czd.gotoacloud.top

[R13] for 计数循环
来源：http://yua.birdmap.top

for i in {1..10}; do echo "$i"; done
来源：http://akq.svipenyu.cn

[R14] C 风格 for
来源：http://yhi.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zbg.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://ijj.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://frp.sweek.top

[R16] until 等待条件
来源：http://sdl.0kj1m.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gvp.mhx1999.top

[R17] 数组定义与取值
来源：http://qjn.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oej.xuetiantiany.cn

[R18] 遍历数组
来源：http://obs.hammf.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xuh.ppjwa.cn

[R19] 数组长度
来源：http://fxk.tianlin.xyz

echo "${#arr[@]}"
来源：http://jdf.smart0.xyz

[R20] 关联数组（字典）
来源：http://kjl.yangfankeji.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gxj.ywan-chungtsiang.top

[R21] 字符串长度
来源：http://xqf.chenjidiqi.icu

echo "${#s}"
来源：http://fzj.fktsv.cn

[R22] 截取子串
来源：http://djp.xuanzx.com

echo "${s:0:5}"
来源：http://yha.zycfv.cn

[R23] 字符串替换
来源：http://qyy.guannengcc.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ahd.yuxming.cn

[R24] 大小写转换
来源：http://gar.gogol.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nob.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://olc.guannengcc.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ymw.xuetiantiany.cn

[R26] 命令替换
来源：http://vtc.zdbjq.cn

now=$(date +%F); echo "$now"
来源：http://bwf.hnxiangtu.top

[R27] 算术展开
来源：http://gwg.0kj1m.cn

echo $((1 + 2 * 3))
来源：http://zld.yvedp.cn

[R28] 浮点运算
来源：http://zai.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://pts.sweek.top

[R29] 定义函数
来源：http://vdm.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kac.xingfuxueyuan.xyz

[R30] 函数返回状态码
来源：http://mkx.cdnleiting.top

f() { return 0; }; f || echo "失败了"
来源：http://buh.aizwys.cn

[R31] 局部变量
来源：http://oyr.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://nym.vqdsnc.cn

[R32] 参数个数校验
来源：http://rcz.hammf.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oua.316326.xyz

[R33] 捕获错误并提示行号
来源：http://fme.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ast.yangfankeji.com

[R34] 退出时清理
来源：http://ayl.nwbrower.top

trap 'rm -f "$tmp"' EXIT
来源：http://zda.zycfv.cn

[R35] 后台执行并等待
来源：http://pju.ivvv.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pay.yuxming.cn

[R36] 并发执行多个任务
来源：http://atd.hammf.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://elp.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://pyh.redwolf501.top

files=$(ls -1)
来源：http://ftp.yongpay.top

[R38] 管道串联
来源：http://ijt.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://aic.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://vct.uphjek.com

cmd > out.log 2>&1
来源：http://esy.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://gug.shzxlz.cn

echo "log" >> out.log
来源：http://kce.xuanzx.com

[R41] 丢弃输出
来源：http://zfg.yj20258888.top

cmd >/dev/null 2>&1
来源：http://xvz.316326.xyz

[R42] 输入重定向
来源：http://gcn.zhoulong.xyz

wc -l < a.txt
来源：http://cls.birdmap.top

[R43] 按名字查找文件
来源：http://crj.xziqi.cn

find . -name "*.log" -type f
来源：http://vps.iojbl.cn

[R44] 按修改时间查找
来源：http://ibh.hfpthk.cn

find . -mtime -7 -type f
来源：http://vlw.jqgufenzy.top

[R45] 批量删除
来源：http://qyq.9152youxi.cn

find . -name "*.tmp" -delete
来源：http://fhb.jiagoushi.top

[R46] 递归替换文件内容
来源：http://ait.9152youxi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uzi.birdmap.top

[R47] sed 单行替换
来源：http://lab.hammf.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lby.jyoumei.cn

[R48] awk 取指定列
来源：http://lmj.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://jki.ybcxt.top

[R49] awk 带条件
来源：http://bsk.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://egw.jqgfzy.top

[R50] awk 求和
来源：http://xci.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://cye.yuanzhike.top

[R51] 排序去重取前几
来源：http://rbx.svipenyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mjf.hnqzz.top

[R52] 统计行数
来源：http://zsq.jianghu66.top

wc -l a.txt
来源：http://ewz.tanke756.top

[R53] 查看文件头与实时尾
来源：http://nej.zhongyouzk.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://czi.pengpengdd.cyou

[R54] 比较两个文件
来源：http://dou.gogol.net.cn

diff a.txt b.txt
来源：http://ebp.hongshengwenyu.top

[R55] 压缩与解压
来源：http://bib.snrcjt.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ogv.ydjk.org.cn

[R56] 远程拷贝
来源：http://zee.sxryk.cn

scp file user@host:/path/
来源：http://pzn.vehdjk.com

[R57] 远程执行命令
来源：http://lhn.ctjpmb.com

ssh user@host 'uptime'
来源：http://cri.zhijiandao.cn

[R58] 下载文件
来源：http://lxl.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lqi.daria6918.cn

[R59] 发 POST JSON
来源：http://nzy.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mwr.quarkkingdee.top

[R60] 只看 HTTP 状态码
来源：http://fys.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ttc.jlsjyb.cn

[R61] 磁盘占用
来源：http://vpt.cqqwz.cn

df -h;  du -sh *
来源：http://gpk.uphjek.com

[R62] 找最占空间的文件
来源：http://zbf.sjlbkw.cn

du -ah . | sort -rh | head -10
来源：http://jhn.redwolf501.top

[R63] 内存与进程
来源：http://jsb.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://bpc.daxiang520.top

[R64] 结束进程
来源：http://oek.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://wmz.xinyue.icu

[R65] 查看端口占用
来源：http://hzo.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ezk.chenjidiqi.icu

[R66] 定时任务
来源：http://xyf.meibo888.top

crontab -e;  crontab -l
来源：http://rvl.ywan-chungtsiang.top

[R67] 生成随机十六进制串
来源：http://ygt.kuanghao11.cn

openssl rand -hex 16
来源：http://tbw.hywenlv.cn

[R68] 计算文件校验值
来源：http://ytd.shanyushiyangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://cuy.pengpengdd.cyou

[R69] 生成随机密码
来源：http://mzg.hnxiangtu.top

head -c 16 /dev/urandom | base64
来源：http://ukz.yj202588.top

[R70] 时间戳与互转
来源：http://rxv.jyoumei.cn

date +%s;  date -d @1700000000
来源：http://quf.jianghu66.top

[R71] 日期格式化
来源：http://pev.shangyingyoupin.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rhe.jinyuanbaomall.cn

[R72] 等待端口就绪
来源：http://rbz.gogol.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://brx.dashuyun.cn

[R73] 分割大日志
来源：http://pqp.nanxinkj.top

split -l 1000 big.log part_
来源：http://rhj.vqdsnc.cn

[R74] 批量重命名
来源：http://foj.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ihn.jinqigfzy.top

[R75] 导出环境变量
来源：http://paw.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://fvo.yueranfly.top

[R76] 使用临时文件
来源：http://fqw.meibo888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hvy.zhoulong.xyz

[R77] 读取用户输入
来源：http://olx.ehwqpu.com

read -rp "请输入: " ans
来源：http://lrb.feifeiyinyue.top

[R78] 交互式菜单
来源：http://tqu.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://obw.hfpthk.cn

[R79] 解析命令行选项
来源：http://pbw.jyoumei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dam.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://chy.ivvv.top

time ./run.sh
来源：http://ips.zhongyouzk.top

================================================================================
来源：http://lvx.yanxiufei.cn

S. C / C++ 专题
来源：http://lmt.fktsv.cn

================================================================================
来源：http://tfd.nanxuanxn.top

[S01] C：Hello World
来源：http://wty.yuxming.cn

#include <stdio.h>
来源：http://hmo.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jzj.chenzaomai.com

[S02] C：变量与格式化输出
来源：http://xtf.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://cli.yfazqb.com

[S03] C：读入整数
来源：http://zav.cqqwz.cn

int x; scanf("%d", &x);
来源：http://blt.yj20258.top

[S04] C：字符串复制
来源：http://spx.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://drz.yuxming.cn

[S05] C：字符串长度
来源：http://eoy.316326.xyz

strlen(s)
来源：http://euh.yonumen.top

[S06] C：字符串比较
来源：http://lws.dianchejie.cn

strcmp(a, b) == 0
来源：http://riy.hywenlv.cn

[S07] C：数组遍历求和
来源：http://pda.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://api.nwbrower.top

[S08] C：动态内存分配与释放
来源：http://tlq.daxiang520.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xey.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://crp.pengpengdd.cyou

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fvq.yj20258.top

[S10] C：指针与解引用
来源：http://ctj.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://nyu.chenzaomai.com

[S11] C：逐行读文件
来源：http://cjc.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://vlr.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kic.guowangkeji.top

fclose(f);
来源：http://ywq.vehdjk.com

[S12] C：写文件
来源：http://fyu.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tzr.sxryk.cn

[S13] C：宏定义
来源：http://siw.wangdashe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bbf.zhiwuduotai.top

[S14] C：枚举
来源：http://xip.chenzaomai.com

enum Color { RED, GREEN, BLUE };
来源：http://mox.hesvh.cn

[S15] C：类型转换
来源：http://ywd.meibo888.top

(double) a / b
来源：http://hco.xuanzx.com

[S16] C：位操作置位
来源：http://ytf.uphjek.com


<!-- 参考信息 -->