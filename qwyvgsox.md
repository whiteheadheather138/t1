代发 wailian999

[Q44] IN 子查询
来源：http://qhh.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jau.zhixingplan.top

[Q45] EXISTS 判断存在
来源：http://egd.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wvb.smart0.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://rjc.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://act.chenjidiqi.icu

[Q47] 与平均值比较
来源：http://smc.xuanzx.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://see.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://kyb.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://irz.jiagoushi.top

SELECT * FROM t WHERE c > 5;
来源：http://yuy.hnqzz.top

[Q49] 更新单行
来源：http://fwo.jiagoushi.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hvs.ehwqpu.com

[Q50] 批量更新
来源：http://ccw.meibo888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yzt.jiagoushi.top

[Q51] 用子查询更新
来源：http://jie.xinyue.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nxs.tarul.cn

[Q52] 删除指定行
来源：http://tlf.yj20258.top

DELETE FROM users WHERE id = 10;
来源：http://wex.ybcxt.top

[Q53] 按条件删除
来源：http://sdi.shuidangran.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bgi.nwbrower.top

[Q54] 清空表
来源：http://aqz.quarkkingdee.top

TRUNCATE TABLE logs;
来源：http://bwu.fehbvm.com

[Q55] 排名（并列占位）
来源：http://yda.ivvv.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mem.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://rzg.vehdjk.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oaa.xingfuxueyuan.xyz

[Q57] 行号
来源：http://knt.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://erj.dianchejie.cn

[Q58] 累计求和
来源：http://xfb.haohaochexian.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nwy.tianlin.xyz

[Q59] 分组内累计
来源：http://svg.feifeiyinyue.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ltq.nanxuanxn.top

[Q60] 取上一行 / 下一行
来源：http://itw.ybcxt.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nye.zdbjq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wko.chenjidiqi.icu

[Q61] 移动平均
来源：http://wqc.jiagoushi.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nvt.cqqwz.cn

[Q62] 分组占比
来源：http://nvp.xingfuxueyuan.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rai.zdbjq.cn

[Q63] 开启事务
来源：http://akb.ydjk.org.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rhn.ybcxt.top

[Q64] 提交事务
来源：http://fvn.yueranfly.top

COMMIT;
来源：http://bvp.kuanghao11.cn

[Q65] 回滚事务
来源：http://wfl.chenlongwang.top

ROLLBACK;
来源：http://kdw.shzxlz.cn

[Q66] 行锁查询
来源：http://zyr.yj20258888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wbq.redwolf501.top

[Q67] 设置隔离级别
来源：http://udg.yuxming.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ziu.yj20258888.top

[Q68] 保存点
来源：http://sqb.jinqigfzy.top

SAVEPOINT sp1;
来源：http://qhv.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://upt.fktsv.cn

[Q69] 查看执行计划
来源：http://ejf.yj20258.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ugy.jinyuanbaomall.cn

[Q70] 更新统计信息
来源：http://zsq.aibaodan.cn

ANALYZE TABLE users;
来源：http://tse.yj202588.top

[Q71] 查看建表语句
来源：http://urt.yongpay.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ame.mhx1999.top

[Q72] 查看索引
来源：http://efv.sysykeji.top

SHOW INDEX FROM users;
来源：http://jls.birdmap.top

[Q73] 查看表状态
来源：http://xug.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jmo.hcnkem.com

[Q74] 强制使用索引
来源：http://xmx.jianghu66.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://adc.hcnkem.com

[Q75] 日期格式化
来源：http://lfl.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ouh.jyoumei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://odx.yj20258.top

[Q76] 按天统计
来源：http://ezt.gzhubu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gom.snrcjt.cn

[Q77] 时间加减
来源：http://afa.jinqigufen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jqf.tianlin.xyz

[Q78] 当前时间
来源：http://zck.nanxinkj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ruc.52xcode.cn

[Q79] 字符串拼接
来源：http://lcj.daria6918.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eve.epnwcf.com

[Q80] 字符串截取
来源：http://xph.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://adk.sjlbkw.cn

[Q81] 字符串替换
来源：http://cgt.quarkkingdee.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rxa.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://feg.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qnj.snrcjt.cn

[Q83] 大小写转换
来源：http://rtk.0kj1m.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ies.fzhhl.top

[Q84] 去除首尾空格
来源：http://lzx.yj20258.top

SELECT TRIM(name) FROM users;
来源：http://lgj.cdnleiting.top

[Q85] 数值取整
来源：http://oud.epnwcf.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gqp.yanxiufei.cn

[Q86] 读取 JSON 字段
来源：http://nfr.xinyue.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gdy.316326.xyz

[Q87] JSON 字段做条件
来源：http://kim.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oxm.pycfn.com

[Q88] 行转列（条件聚合）
来源：http://zkm.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qcl.c1oappe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bqk.jqgfzy.top

[Q89] 判断表是否存在
来源：http://cst.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ssf.yonumen.top

[Q90] 生成序号列
来源：http://for.zycfv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://utw.andypj.xyz

================================================================================
来源：http://aki.hcnkem.com

R. Bash 专题
来源：http://olg.sweek.top

================================================================================
来源：http://adk.uphjek.com

[R01] shebang 与严格模式
来源：http://zxm.ywan-chungtsiang.top

#!/usr/bin/env bash
来源：http://vnj.yanxiufei.cn

set -euo pipefail
来源：http://akv.bjfxy.top

[R02] 变量赋值与使用
来源：http://veg.svipenyu.cn

name="Tom"; echo "$name"
来源：http://nmu.jlsjyb.cn

[R03] 只读变量
来源：http://ahm.ehwqpu.com

readonly PI=3.14
来源：http://rjf.jlsjyb.cn

[R04] 位置参数
来源：http://fio.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ler.ydzc1.top

[R05] 参数默认值
来源：http://gxa.9152youxi.cn

name="${1:-default}"
来源：http://oyt.cheryme.top

[R06] 判断命令是否存在
来源：http://csd.jlsjyb.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yvs.nanxinkj.top

[R07] if 判断文件
来源：http://tdx.zdbjq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mak.ywan-chungtsiang.top

[R08] 数值比较
来源：http://kcd.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://quc.fanxiaobao.xyz

[R09] 字符串比较
来源：http://mlw.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fqs.hesvh.cn

[R10] 正则匹配
来源：http://hqj.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://byx.zhiwuduotai.top

[R11] case 多分支
来源：http://nfa.zhengqikj.top

case "$1" in
来源：http://fjk.hongshengwenyu.top

start) echo "启动" ;;
来源：http://vhw.sxryk.cn

stop)  echo "停止" ;;
来源：http://mmn.xylfe.cn

*)     echo "未知命令" ;;
来源：http://elm.andypj.xyz

esac
来源：http://mjw.yongpay.top

[R12] for 遍历文件
来源：http://yvl.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://knw.andypj.xyz

[R13] for 计数循环
来源：http://tta.zhijiandao.cn

for i in {1..10}; do echo "$i"; done
来源：http://gry.snrcjt.cn

[R14] C 风格 for
来源：http://xsf.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dhq.bjfxy.top

[R15] while 逐行读文件
来源：http://vic.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jap.tianlin.xyz

[R16] until 等待条件
来源：http://qej.bbcook.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tue.jqgufenzy.top

[R17] 数组定义与取值
来源：http://hdd.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://zjd.hammf.cn

[R18] 遍历数组
来源：http://ywz.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xqt.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://sal.yfazqb.com

echo "${#arr[@]}"
来源：http://rwr.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://snn.xinyue.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jge.dashuyun.cn

[R21] 字符串长度
来源：http://qbh.pycfn.com

echo "${#s}"
来源：http://wks.ehwqpu.com

[R22] 截取子串
来源：http://qca.feifeiyinyue.top

echo "${s:0:5}"
来源：http://pig.9152youxi.cn

[R23] 字符串替换
来源：http://roq.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qiz.sweek.top

[R24] 大小写转换
来源：http://rhx.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://jgl.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://ksc.zdbjq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://avm.ydzc1.top

[R26] 命令替换
来源：http://xpc.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://nwi.xziqi.cn

[R27] 算术展开
来源：http://zxs.jianghu66.top

echo $((1 + 2 * 3))
来源：http://kex.zdqjudy.top

[R28] 浮点运算
来源：http://cuv.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://xhf.zhengqikj.top

[R29] 定义函数
来源：http://dko.yvedp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bkc.yj20258.top

[R30] 函数返回状态码
来源：http://ckv.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://yty.sweek.top

[R31] 局部变量
来源：http://fav.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://avl.xinyue.icu

[R32] 参数个数校验
来源：http://wcu.ybcxt.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dzw.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://quy.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vyi.0kj1m.cn

[R34] 退出时清理
来源：http://vob.nwbrower.top

trap 'rm -f "$tmp"' EXIT
来源：http://xxx.pengpengdd.cyou

[R35] 后台执行并等待
来源：http://aoo.nanxinkj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vtk.yangfankeji.com

[R36] 并发执行多个任务
来源：http://jsd.xinyue.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jsb.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://zdi.sweek.top

files=$(ls -1)
来源：http://xnp.vqdsnc.cn

[R38] 管道串联
来源：http://vng.bjfxy.top

cat a.txt | grep -i error | wc -l
来源：http://tsd.aibaodan.cn

[R39] 重定向标准输出与错误
来源：http://nvx.tian-w.cn

cmd > out.log 2>&1
来源：http://tud.xylfe.cn

[R40] 追加写日志
来源：http://mpz.chenjidiqi.icu

echo "log" >> out.log
来源：http://ich.jqgufenzy.top

[R41] 丢弃输出
来源：http://bzq.smart0.xyz

cmd >/dev/null 2>&1
来源：http://gnf.tarul.cn

[R42] 输入重定向
来源：http://cae.kuanghao11.cn

wc -l < a.txt
来源：http://jwl.xziqi.cn

[R43] 按名字查找文件
来源：http://nky.hammf.cn

find . -name "*.log" -type f
来源：http://idc.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://ali.ehwqpu.com

find . -mtime -7 -type f
来源：http://jco.xingfuxueyuan.xyz

[R45] 批量删除
来源：http://thy.aizwys.cn

find . -name "*.tmp" -delete
来源：http://did.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://dyx.hnxiangtu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fua.zhiwuduotai.top

[R47] sed 单行替换
来源：http://mip.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://qkb.fengsongda.top

[R48] awk 取指定列
来源：http://ynp.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://ago.zhixingplan.top

[R49] awk 带条件
来源：http://set.9152youxi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ilp.mhx1999.top

[R50] awk 求和
来源：http://rmc.cashguo.top

awk '{s += $2} END {print s}' a.txt
来源：http://nhz.mhx1999.top

[R51] 排序去重取前几
来源：http://kuc.fzhhl.top

sort a.txt | uniq -c | sort -rn | head
来源：http://oht.yj202588.top

[R52] 统计行数
来源：http://kwn.gogol.net.cn

wc -l a.txt
来源：http://mke.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://gpe.ehwqpu.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iya.yj20258.top

[R54] 比较两个文件
来源：http://qhy.dashuyun.cn

diff a.txt b.txt
来源：http://npf.xylfe.cn

[R55] 压缩与解压
来源：http://mrn.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://aib.gogol.net.cn

[R56] 远程拷贝
来源：http://iqi.ppjwa.cn

scp file user@host:/path/
来源：http://frf.zhengqikj.top

[R57] 远程执行命令
来源：http://roj.nwbrower.top

ssh user@host 'uptime'
来源：http://okb.dashuyun.cn

[R58] 下载文件
来源：http://aig.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rxn.dashuyun.cn

[R59] 发 POST JSON
来源：http://rix.zhoulong.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uaq.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://jbf.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qew.ehwqpu.com

[R61] 磁盘占用
来源：http://xyj.redwolf501.top

df -h;  du -sh *
来源：http://vbj.ybcxt.top

[R62] 找最占空间的文件
来源：http://okn.vqdsnc.cn

du -ah . | sort -rh | head -10
来源：http://udh.smart0.xyz

[R63] 内存与进程
来源：http://rhg.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://vvo.ctjpmb.com

[R64] 结束进程
来源：http://vye.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://rum.havefunace.top

[R65] 查看端口占用
来源：http://ccs.yangfankeji.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gjw.jianghu66.top

[R66] 定时任务
来源：http://jqo.shuidangran.top

crontab -e;  crontab -l
来源：http://sii.yj20258.top

[R67] 生成随机十六进制串
来源：http://zfi.9152youxi.cn

openssl rand -hex 16
来源：http://qci.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://crn.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://kvg.ppjwa.cn

[R69] 生成随机密码
来源：http://rsq.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://iiy.yueranfly.top

[R70] 时间戳与互转
来源：http://xjo.shzxlz.cn

date +%s;  date -d @1700000000
来源：http://qjh.fehbvm.com

[R71] 日期格式化
来源：http://tyi.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gdi.zdqjudy.top

[R72] 等待端口就绪
来源：http://otl.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://oug.chenzaomai.com

[R73] 分割大日志
来源：http://sao.yonumen.top

split -l 1000 big.log part_
来源：http://kul.epnwcf.com

[R74] 批量重命名
来源：http://ebg.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rha.yuanzhike.top

[R75] 导出环境变量
来源：http://uaw.gotoacloud.top

export PATH="$HOME/bin:$PATH"
来源：http://ytq.smart0.xyz

[R76] 使用临时文件
来源：http://tqi.sysykeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://apn.xinyue.icu

[R77] 读取用户输入
来源：http://ymq.0kj1m.cn

read -rp "请输入: " ans
来源：http://skr.iojbl.cn

[R78] 交互式菜单
来源：http://pnz.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://spf.tarul.cn

[R79] 解析命令行选项
来源：http://xut.316326.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gsi.yongpay.top

[R80] 查看脚本执行耗时
来源：http://mdi.jianghu66.top

time ./run.sh
来源：http://shg.haohaochexian.top

================================================================================
来源：http://nfs.yuanzhike.top

S. C / C++ 专题
来源：http://mih.zycfv.cn

================================================================================
来源：http://oqz.nwbrower.top

[S01] C：Hello World
来源：http://oax.cdnleiting.top

#include <stdio.h>
来源：http://hpo.andypj.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://dux.jinyuanbaomall.cn

[S02] C：变量与格式化输出
来源：http://xcz.kuanghao11.cn

int a = 10; printf("%d\n", a);
来源：http://fxm.tian-w.cn

[S03] C：读入整数
来源：http://skx.aibaodan.cn

int x; scanf("%d", &x);
来源：http://tpa.fktsv.cn

[S04] C：字符串复制
来源：http://mdr.iojbl.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nhq.fengsongda.top

[S05] C：字符串长度
来源：http://fvz.fengsongda.top

strlen(s)
来源：http://ngf.meibo888.top

[S06] C：字符串比较
来源：http://fhb.cdnleiting.top

strcmp(a, b) == 0
来源：http://nyg.mhx1999.top

[S07] C：数组遍历求和
来源：http://mgi.zhongyouzk.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hfz.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://mpt.xuanzx.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://edm.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://nxk.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ehc.zhoulong.xyz

[S10] C：指针与解引用
来源：http://gkw.xuanzx.com

int *p = &a;  *p = 5;
来源：http://shj.sjlbkw.cn

[S11] C：逐行读文件
来源：http://jin.havefunace.top

FILE *f = fopen("a.txt", "r");
来源：http://uxd.jiagoushi.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://uic.uphjek.com

fclose(f);
来源：http://ukr.jlsjyb.cn

[S12] C：写文件
来源：http://vfu.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xzo.jyoumei.cn

[S13] C：宏定义
来源：http://lwx.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kpk.fengsongda.top

[S14] C：枚举
来源：http://whs.nanxuanxn.top


<!-- 参考信息 -->