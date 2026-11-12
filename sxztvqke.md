代发 wailian999

[Q44] IN 子查询
来源：http://lht.cucudq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kmh.jinyuanbaomall.cn

[Q45] EXISTS 判断存在
来源：http://lbw.xuanzx.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pvb.nwbrower.top

[Q46] NOT EXISTS 判断不存在
来源：http://bir.yj20258888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://seg.yangfankeji.com

[Q47] 与平均值比较
来源：http://nkb.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oos.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://drm.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://plb.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://tsw.shanyushiyangtech.top

[Q49] 更新单行
来源：http://zgv.ehwqpu.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tbz.nwbrower.top

[Q50] 批量更新
来源：http://pth.jyoumei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://avf.yvedp.cn

[Q51] 用子查询更新
来源：http://ogq.zycfv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cze.tanke756.top

[Q52] 删除指定行
来源：http://ave.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://hch.cashguo.top

[Q53] 按条件删除
来源：http://zjj.yvedp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qzj.vqdsnc.cn

[Q54] 清空表
来源：http://vwg.birdmap.top

TRUNCATE TABLE logs;
来源：http://aby.fengsongda.top

[Q55] 排名（并列占位）
来源：http://kxd.havefunace.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wjx.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://dkp.zdqjudy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iba.fengsongda.top

[Q57] 行号
来源：http://fjj.jqgfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sur.316326.xyz

[Q58] 累计求和
来源：http://vqe.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pxt.gotoacloud.top

[Q59] 分组内累计
来源：http://jkd.andypj.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wym.yj20258.top

[Q60] 取上一行 / 下一行
来源：http://khb.jlsjyb.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hwv.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zxc.haohaochexian.top

[Q61] 移动平均
来源：http://lzm.cashguo.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://syz.shzxlz.cn

[Q62] 分组占比
来源：http://qeu.hywenlv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jhs.zhaomingkeji.xyz

[Q63] 开启事务
来源：http://fjn.gotoacloud.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qvq.cashguo.top

[Q64] 提交事务
来源：http://llx.xuanzx.com

COMMIT;
来源：http://apd.ivvv.top

[Q65] 回滚事务
来源：http://whb.haohaochexian.top

ROLLBACK;
来源：http://zqf.svipenyu.cn

[Q66] 行锁查询
来源：http://iam.epnwcf.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ndi.zhongyouzk.top

[Q67] 设置隔离级别
来源：http://mqr.zhongyouzk.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://njv.sjlbkw.cn

[Q68] 保存点
来源：http://pqw.jyoumei.cn

SAVEPOINT sp1;
来源：http://cvc.jyoumei.cn

ROLLBACK TO sp1;
来源：http://pfv.yanxiufei.cn

[Q69] 查看执行计划
来源：http://tdx.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sbp.xziqi.cn

[Q70] 更新统计信息
来源：http://bib.ydzc1.top

ANALYZE TABLE users;
来源：http://wal.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://ixm.hysaishi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ilp.redwolf501.top

[Q72] 查看索引
来源：http://oxj.svipenyu.cn

SHOW INDEX FROM users;
来源：http://ddv.zdbjq.cn

[Q73] 查看表状态
来源：http://dip.zhongyouzk.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qkj.uphjek.com

[Q74] 强制使用索引
来源：http://tfe.zhijiandao.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lmn.chenlongwang.top

[Q75] 日期格式化
来源：http://xoz.yj20258.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dgb.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yxl.aizwys.cn

[Q76] 按天统计
来源：http://psl.chenjidiqi.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sdr.shanyushiyangtech.top

[Q77] 时间加减
来源：http://rxq.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sky.haohaochexian.top

[Q78] 当前时间
来源：http://rhs.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bpi.nwbrower.top

[Q79] 字符串拼接
来源：http://pdm.daria6918.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lte.yj20258888.top

[Q80] 字符串截取
来源：http://pvw.jinqigufen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xux.mhx1999.top

[Q81] 字符串替换
来源：http://tci.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://prn.andypj.xyz

[Q82] 字符长度与字节长度
来源：http://lsw.nwbrower.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pxk.sjlbkw.cn

[Q83] 大小写转换
来源：http://vti.ctjpmb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kgg.9152youxi.cn

[Q84] 去除首尾空格
来源：http://tho.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://gaz.shangyingyoupin.top

[Q85] 数值取整
来源：http://nqz.hfpthk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://njz.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://qmd.gaohongyu789.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wau.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://brr.dashuyun.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://muw.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://auy.yanxiufei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dgr.hywenlv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://quj.fzhhl.top

[Q89] 判断表是否存在
来源：http://fxj.ybcxt.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dqm.tianlin.xyz

[Q90] 生成序号列
来源：http://ahx.svipenyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fti.wangshuangyany.cn

================================================================================
来源：http://svm.jianghu66.top

R. Bash 专题
来源：http://bvv.pengpengdd.cyou

================================================================================
来源：http://mqj.316326.xyz

[R01] shebang 与严格模式
来源：http://sev.cdnleiting.top

#!/usr/bin/env bash
来源：http://txv.hammf.cn

set -euo pipefail
来源：http://rok.zdqjudy.top

[R02] 变量赋值与使用
来源：http://zbb.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://yky.zhengqikj.top

[R03] 只读变量
来源：http://gac.hysaishi.cn

readonly PI=3.14
来源：http://llx.316326.xyz

[R04] 位置参数
来源：http://anf.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eor.gzhubu.top

[R05] 参数默认值
来源：http://rcm.jlsjyb.cn

name="${1:-default}"
来源：http://ytx.cdnleiting.top

[R06] 判断命令是否存在
来源：http://sxi.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uvi.chenlongwang.top

[R07] if 判断文件
来源：http://whh.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lsp.quarkkingdee.top

[R08] 数值比较
来源：http://lfy.52xcode.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://spt.zhaomingkeji.xyz

[R09] 字符串比较
来源：http://zdh.jinqigfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://akl.yj202588.top

[R10] 正则匹配
来源：http://eyo.shzxlz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ijq.epnwcf.com

[R11] case 多分支
来源：http://htt.zycfv.cn

case "$1" in
来源：http://fak.hysaishi.cn

start) echo "启动" ;;
来源：http://bxw.52xcode.cn

stop)  echo "停止" ;;
来源：http://ios.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://iaw.hongshengwenyu.top

esac
来源：http://fnw.sysykeji.top

[R12] for 遍历文件
来源：http://kko.zhengqikj.top

for f in *.txt; do echo "$f"; done
来源：http://tap.ydzc1.top

[R13] for 计数循环
来源：http://koh.yonumen.top

for i in {1..10}; do echo "$i"; done
来源：http://gxg.redwolf501.top

[R14] C 风格 for
来源：http://xvp.wangshuangyany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://odp.yanxiufei.cn

[R15] while 逐行读文件
来源：http://icl.aibaodan.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://btj.bjfxy.top

[R16] until 等待条件
来源：http://njn.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://loh.yonumen.top

[R17] 数组定义与取值
来源：http://cpk.iojbl.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lmn.hywenlv.cn

[R18] 遍历数组
来源：http://ywp.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://okh.c1oappe.top

[R19] 数组长度
来源：http://pik.xylfe.cn

echo "${#arr[@]}"
来源：http://mze.ppjwa.cn

[R20] 关联数组（字典）
来源：http://nbh.smart0.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hvc.kuanghao11.cn

[R21] 字符串长度
来源：http://xbt.redwolf501.top

echo "${#s}"
来源：http://trx.ydjk.org.cn

[R22] 截取子串
来源：http://igh.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://mnm.tian-w.cn

[R23] 字符串替换
来源：http://zne.fengsongda.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ydm.jiagoushi.top

[R24] 大小写转换
来源：http://pkp.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://ydp.jinghuilouyu.cn

[R25] 去后缀 / 去前缀
来源：http://kms.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nrc.chenzaomai.com

[R26] 命令替换
来源：http://oqx.jyoumei.cn

now=$(date +%F); echo "$now"
来源：http://yjo.jlsjyb.cn

[R27] 算术展开
来源：http://wrg.shanyushiyangtech.top

echo $((1 + 2 * 3))
来源：http://lbu.c1oappe.top

[R28] 浮点运算
来源：http://ere.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://vui.meibo888.top

[R29] 定义函数
来源：http://pxy.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ysc.chenzaomai.com

[R30] 函数返回状态码
来源：http://uks.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://fhu.guowangkeji.top

[R31] 局部变量
来源：http://tzf.zhiwuduotai.top

f() { local x=1; echo "$x"; }
来源：http://slt.jinqigufen.top

[R32] 参数个数校验
来源：http://cts.sjlbkw.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nzh.iojbl.cn

[R33] 捕获错误并提示行号
来源：http://dgj.sysykeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hte.sxryk.cn

[R34] 退出时清理
来源：http://vyx.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://kuv.tarul.cn

[R35] 后台执行并等待
来源：http://rln.redwolf501.top

sleep 5 & pid=$!; wait "$pid"
来源：http://imn.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://twa.hesvh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mxe.nanxinkj.top

[R37] 把输出赋给变量
来源：http://ysd.hnxiangtu.top

files=$(ls -1)
来源：http://uyr.guowangkeji.top

[R38] 管道串联
来源：http://zik.yuanzhike.top

cat a.txt | grep -i error | wc -l
来源：http://drp.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://meb.pycfn.com

cmd > out.log 2>&1
来源：http://hxy.hongshengwenyu.top

[R40] 追加写日志
来源：http://idr.jlsjyb.cn

echo "log" >> out.log
来源：http://oci.gaohongyu789.top

[R41] 丢弃输出
来源：http://tpp.ehwqpu.com

cmd >/dev/null 2>&1
来源：http://gdz.redwolf501.top

[R42] 输入重定向
来源：http://kcr.aibaodan.cn

wc -l < a.txt
来源：http://tao.fzhhl.top

[R43] 按名字查找文件
来源：http://tiy.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://box.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://krg.snrcjt.cn

find . -mtime -7 -type f
来源：http://gps.jinqigfzy.top

[R45] 批量删除
来源：http://wwk.tian-w.cn

find . -name "*.tmp" -delete
来源：http://tru.smart0.xyz

[R46] 递归替换文件内容
来源：http://duc.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dza.svipenyu.cn

[R47] sed 单行替换
来源：http://wdk.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xqx.hysaishi.cn

[R48] awk 取指定列
来源：http://rom.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://abu.andypj.xyz

[R49] awk 带条件
来源：http://vjs.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://brw.hfpthk.cn

[R50] awk 求和
来源：http://axe.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://ymx.gotoacloud.top

[R51] 排序去重取前几
来源：http://jsb.yj20258.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ufv.sxryk.cn

[R52] 统计行数
来源：http://dvb.pengpengdd.cyou

wc -l a.txt
来源：http://smp.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://mzq.nwbrower.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://seh.fzhhl.top

[R54] 比较两个文件
来源：http://jdu.yj20258888.top

diff a.txt b.txt
来源：http://lvu.yangfankeji.com

[R55] 压缩与解压
来源：http://sgz.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://csi.uphjek.com

[R56] 远程拷贝
来源：http://vde.feifeiyinyue.top

scp file user@host:/path/
来源：http://eiv.xinyue.icu

[R57] 远程执行命令
来源：http://ytt.chenjidiqi.icu

ssh user@host 'uptime'
来源：http://dii.yangfankeji.com

[R58] 下载文件
来源：http://kvy.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qhb.uphjek.com

[R59] 发 POST JSON
来源：http://flw.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yky.shzxlz.cn

[R60] 只看 HTTP 状态码
来源：http://wsp.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tln.epnwcf.com

[R61] 磁盘占用
来源：http://bjv.zhaomingkeji.xyz

df -h;  du -sh *
来源：http://jeu.yj20258888.top

[R62] 找最占空间的文件
来源：http://iun.cashguo.top

du -ah . | sort -rh | head -10
来源：http://yfn.hywenlv.cn

[R63] 内存与进程
来源：http://uym.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://klc.jinghuilouyu.cn

[R64] 结束进程
来源：http://skv.hammf.cn

kill -9 $(pgrep -f app.py)
来源：http://ulf.shangyingyoupin.top

[R65] 查看端口占用
来源：http://hxu.zdbjq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fvm.quarkkingdee.top

[R66] 定时任务
来源：http://dqn.ydjk.org.cn

crontab -e;  crontab -l
来源：http://mcb.nwbrower.top

[R67] 生成随机十六进制串
来源：http://ogb.cdnleiting.top

openssl rand -hex 16
来源：http://noy.yonumen.top

[R68] 计算文件校验值
来源：http://ppc.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://plb.zycfv.cn

[R69] 生成随机密码
来源：http://bym.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://kjg.fktsv.cn

[R70] 时间戳与互转
来源：http://osa.sysykeji.top

date +%s;  date -d @1700000000
来源：http://rvq.chenjidiqi.icu

[R71] 日期格式化
来源：http://jjf.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://urh.ivvv.top

[R72] 等待端口就绪
来源：http://jmu.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://quu.hammf.cn

[R73] 分割大日志
来源：http://vtp.redwolf501.top

split -l 1000 big.log part_
来源：http://gua.316326.xyz

[R74] 批量重命名
来源：http://lgr.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wnb.yueranfly.top

[R75] 导出环境变量
来源：http://myx.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://imb.sufxvd.cn

[R76] 使用临时文件
来源：http://iho.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uld.cqqwz.cn

[R77] 读取用户输入
来源：http://qho.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://cyf.gotoacloud.top

[R78] 交互式菜单
来源：http://uxk.ydzc1.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gmb.yfazqb.com

[R79] 解析命令行选项
来源：http://fcs.pycfn.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tys.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://sdq.jlsjyb.cn

time ./run.sh
来源：http://mgr.aizwys.cn

================================================================================
来源：http://suq.zdqjudy.top

S. C / C++ 专题
来源：http://txi.hongshengwenyu.top

================================================================================
来源：http://sok.gzhubu.top

[S01] C：Hello World
来源：http://nbo.shangyingyoupin.top

#include <stdio.h>
来源：http://piv.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qlg.hammf.cn

[S02] C：变量与格式化输出
来源：http://jmq.hongshengwenyu.top

int a = 10; printf("%d\n", a);
来源：http://edd.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://uny.ctjpmb.com

int x; scanf("%d", &x);
来源：http://ifw.smart0.xyz

[S04] C：字符串复制
来源：http://evi.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://juj.ydjk.org.cn

[S05] C：字符串长度
来源：http://jva.zhaomingkeji.xyz

strlen(s)
来源：http://uts.ydjk.org.cn

[S06] C：字符串比较
来源：http://mxz.yj20258888.top

strcmp(a, b) == 0
来源：http://lfj.chenzaomai.com

[S07] C：数组遍历求和
来源：http://whh.wangshuangyany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nau.haohaochexian.top

[S08] C：动态内存分配与释放
来源：http://hdv.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mrp.gogol.net.cn

[S09] C：结构体定义与初始化
来源：http://gfo.cqqwz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vlh.yonumen.top

[S10] C：指针与解引用
来源：http://xij.yongpay.top

int *p = &a;  *p = 5;
来源：http://puk.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://qva.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://byd.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nvw.cashguo.top

fclose(f);
来源：http://kcy.bjfxy.top

[S12] C：写文件
来源：http://zkf.guowangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iai.hcnkem.com

[S13] C：宏定义
来源：http://ttd.yangfankeji.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://etx.zycfv.cn

[S14] C：枚举
来源：http://yet.shangyingyoupin.top


<!-- 参考信息 -->