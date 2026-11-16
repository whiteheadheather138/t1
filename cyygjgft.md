代发 wailian999

[Q44] IN 子查询
来源：http://vzq.jlsjyb.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cew.cucudq.cn

[Q45] EXISTS 判断存在
来源：http://pad.zhiwuduotai.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sgq.yongpay.top

[Q46] NOT EXISTS 判断不存在
来源：http://gvx.ehwqpu.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wol.tanke756.top

[Q47] 与平均值比较
来源：http://cwg.cqqwz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://obc.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://ekf.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hey.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://ksx.jqgufenzy.top

[Q49] 更新单行
来源：http://hsb.cqqwz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bzn.pycfn.com

[Q50] 批量更新
来源：http://svi.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nhd.nanxuanxn.top

[Q51] 用子查询更新
来源：http://exr.ywan-chungtsiang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nat.tian-w.cn

[Q52] 删除指定行
来源：http://sde.yfazqb.com

DELETE FROM users WHERE id = 10;
来源：http://aak.fanxiaobao.xyz

[Q53] 按条件删除
来源：http://xmj.jiagoushi.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://buo.yanxiufei.cn

[Q54] 清空表
来源：http://nqt.vqdsnc.cn

TRUNCATE TABLE logs;
来源：http://ukw.feifeiyinyue.top

[Q55] 排名（并列占位）
来源：http://qow.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lsy.xylfe.cn

[Q56] 密集排名（并列不占位）
来源：http://von.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hbu.chenzaomai.com

[Q57] 行号
来源：http://moe.sufxvd.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rdm.ydjk.org.cn

[Q58] 累计求和
来源：http://ark.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vxv.guannengcc.top

[Q59] 分组内累计
来源：http://yqg.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ncr.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://drb.quarkkingdee.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tzq.gzhubu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hev.pycfn.com

[Q61] 移动平均
来源：http://dra.zhijiandao.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://otq.chenzaomai.com

[Q62] 分组占比
来源：http://sws.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yxk.ivvv.top

[Q63] 开启事务
来源：http://nwj.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dlg.yvedp.cn

[Q64] 提交事务
来源：http://irh.fengsongda.top

COMMIT;
来源：http://cbf.guowangkeji.top

[Q65] 回滚事务
来源：http://jll.hesvh.cn

ROLLBACK;
来源：http://pqb.iojbl.cn

[Q66] 行锁查询
来源：http://kbt.epnwcf.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://trf.jqgfzy.top

[Q67] 设置隔离级别
来源：http://far.cashguo.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jjp.gzhubu.top

[Q68] 保存点
来源：http://uyj.yj20258888.top

SAVEPOINT sp1;
来源：http://gvm.nanxuanxn.top

ROLLBACK TO sp1;
来源：http://cph.snrcjt.cn

[Q69] 查看执行计划
来源：http://man.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nfq.jlsjyb.cn

[Q70] 更新统计信息
来源：http://buv.ctjpmb.com

ANALYZE TABLE users;
来源：http://meu.jianghu66.top

[Q71] 查看建表语句
来源：http://dbc.hongshengwenyu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mpi.zhixingplan.top

[Q72] 查看索引
来源：http://ygq.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://eqf.fehbvm.com

[Q73] 查看表状态
来源：http://uzr.wangdashe.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vjw.uphjek.com

[Q74] 强制使用索引
来源：http://ska.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tzg.hnqzz.top

[Q75] 日期格式化
来源：http://rvn.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://piz.daxiang520.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jpv.andypj.xyz

[Q76] 按天统计
来源：http://xek.hysaishi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mww.cqqwz.cn

[Q77] 时间加减
来源：http://ehv.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zvu.cdnleiting.top

[Q78] 当前时间
来源：http://plf.ivvv.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ahg.xziqi.cn

[Q79] 字符串拼接
来源：http://thb.shanyushiyangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://atf.smart0.xyz

[Q80] 字符串截取
来源：http://zvs.hfpthk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://czq.tanke756.top

[Q81] 字符串替换
来源：http://tjd.yuxming.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xni.shzxlz.cn

[Q82] 字符长度与字节长度
来源：http://mkk.daria6918.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vda.xuanzx.com

[Q83] 大小写转换
来源：http://mrx.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vfn.chenzaomai.com

[Q84] 去除首尾空格
来源：http://bay.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://rfp.ivvv.top

[Q85] 数值取整
来源：http://sav.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tny.yuxming.cn

[Q86] 读取 JSON 字段
来源：http://gon.mhx1999.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://owx.guowangkeji.top

[Q87] JSON 字段做条件
来源：http://aeo.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xwo.nwbrower.top

[Q88] 行转列（条件聚合）
来源：http://jnh.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kex.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uku.zhijiandao.cn

[Q89] 判断表是否存在
来源：http://bub.ydzc1.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wne.jqgfzy.top

[Q90] 生成序号列
来源：http://oim.zdbjq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xlv.andypj.xyz

================================================================================
来源：http://flm.mhx1999.top

R. Bash 专题
来源：http://fmh.tian-w.cn

================================================================================
来源：http://ant.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://etc.ivvv.top

#!/usr/bin/env bash
来源：http://sax.xingfuxueyuan.xyz

set -euo pipefail
来源：http://ewj.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://rpi.xuetiantiany.cn

name="Tom"; echo "$name"
来源：http://vto.xingfuxueyuan.xyz

[R03] 只读变量
来源：http://sbz.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://kkp.daria6918.cn

[R04] 位置参数
来源：http://bas.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rai.shangyingyoupin.top

[R05] 参数默认值
来源：http://psc.zdqjudy.top

name="${1:-default}"
来源：http://yut.hnqzz.top

[R06] 判断命令是否存在
来源：http://gud.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://asp.hnqzz.top

[R07] if 判断文件
来源：http://pfd.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nxz.cheryme.top

[R08] 数值比较
来源：http://qat.dashuyun.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://soz.gogol.net.cn

[R09] 字符串比较
来源：http://csz.zhijiandao.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://glr.zhongyouzk.top

[R10] 正则匹配
来源：http://kdd.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wdu.jianghu66.top

[R11] case 多分支
来源：http://szh.yanxiufei.cn

case "$1" in
来源：http://ugg.yangfankeji.com

start) echo "启动" ;;
来源：http://vsn.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://tzx.snrcjt.cn

*)     echo "未知命令" ;;
来源：http://lox.smart0.xyz

esac
来源：http://xbk.snrcjt.cn

[R12] for 遍历文件
来源：http://pvp.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://boz.aibaodan.cn

[R13] for 计数循环
来源：http://xio.hnqzz.top

for i in {1..10}; do echo "$i"; done
来源：http://eos.daxiang520.top

[R14] C 风格 for
来源：http://oai.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://plo.uphjek.com

[R15] while 逐行读文件
来源：http://wzc.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bds.xuetiantiany.cn

[R16] until 等待条件
来源：http://bgv.cdnleiting.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gnx.jinqigufen.top

[R17] 数组定义与取值
来源：http://una.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://vwr.yj20258.top

[R18] 遍历数组
来源：http://ihc.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hbp.c1oappe.top

[R19] 数组长度
来源：http://ttn.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://jia.svipenyu.cn

[R20] 关联数组（字典）
来源：http://btq.fzhhl.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jkb.shangyingyoupin.top

[R21] 字符串长度
来源：http://blv.nwbrower.top

echo "${#s}"
来源：http://qcx.yj20258.top

[R22] 截取子串
来源：http://ozz.iojbl.cn

echo "${s:0:5}"
来源：http://kka.daxiang520.top

[R23] 字符串替换
来源：http://tpt.ppjwa.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://use.sjlbkw.cn

[R24] 大小写转换
来源：http://jqs.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://ccc.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://til.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vgv.nwbrower.top

[R26] 命令替换
来源：http://eft.xziqi.cn

now=$(date +%F); echo "$now"
来源：http://yfh.guowangkeji.top

[R27] 算术展开
来源：http://wwr.cdnleiting.top

echo $((1 + 2 * 3))
来源：http://uvc.hesvh.cn

[R28] 浮点运算
来源：http://tcb.sufxvd.cn

echo "scale=2; 10/3" | bc
来源：http://jev.yj202588.top

[R29] 定义函数
来源：http://jrq.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wkk.xuanzx.com

[R30] 函数返回状态码
来源：http://cqg.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://nza.andypj.xyz

[R31] 局部变量
来源：http://ooz.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://zjm.nanxuanxn.top

[R32] 参数个数校验
来源：http://pek.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wmx.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://gqv.hcnkem.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wib.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://ega.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://pav.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://ukm.hongshengwenyu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://aem.dianchejie.cn

[R36] 并发执行多个任务
来源：http://kws.jinyuanbaomall.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nsu.smart0.xyz

[R37] 把输出赋给变量
来源：http://pvo.hesvh.cn

files=$(ls -1)
来源：http://gnq.zycfv.cn

[R38] 管道串联
来源：http://leu.aizwys.cn

cat a.txt | grep -i error | wc -l
来源：http://bil.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://ilx.xziqi.cn

cmd > out.log 2>&1
来源：http://uww.xuetiantiany.cn

[R40] 追加写日志
来源：http://dnz.jlsjyb.cn

echo "log" >> out.log
来源：http://ene.shzxlz.cn

[R41] 丢弃输出
来源：http://mhg.gotoacloud.top

cmd >/dev/null 2>&1
来源：http://lew.xziqi.cn

[R42] 输入重定向
来源：http://ljl.9152youxi.cn

wc -l < a.txt
来源：http://isj.yanxiufei.cn

[R43] 按名字查找文件
来源：http://vkz.yanxiufei.cn

find . -name "*.log" -type f
来源：http://sjr.havefunace.top

[R44] 按修改时间查找
来源：http://cgs.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://foi.yvedp.cn

[R45] 批量删除
来源：http://mxk.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://tes.jiagoushi.top

[R46] 递归替换文件内容
来源：http://tpp.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jkz.xuanzx.com

[R47] sed 单行替换
来源：http://gja.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gsm.nanxuanxn.top

[R48] awk 取指定列
来源：http://ysx.yongpay.top

awk '{print $1, $3}' a.txt
来源：http://izc.yonumen.top

[R49] awk 带条件
来源：http://npt.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fhy.birdmap.top

[R50] awk 求和
来源：http://hub.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vmd.kuanghao11.cn

[R51] 排序去重取前几
来源：http://tob.fzhhl.top

sort a.txt | uniq -c | sort -rn | head
来源：http://djz.xingfuxueyuan.xyz

[R52] 统计行数
来源：http://qaq.hesvh.cn

wc -l a.txt
来源：http://drh.havefunace.top

[R53] 查看文件头与实时尾
来源：http://xph.zhoulong.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fik.tarul.cn

[R54] 比较两个文件
来源：http://xoe.epnwcf.com

diff a.txt b.txt
来源：http://rqf.chenjidiqi.icu

[R55] 压缩与解压
来源：http://iuo.chenjidiqi.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hgh.tian-w.cn

[R56] 远程拷贝
来源：http://qyf.sysykeji.top

scp file user@host:/path/
来源：http://hch.0kj1m.cn

[R57] 远程执行命令
来源：http://skr.tianlin.xyz

ssh user@host 'uptime'
来源：http://chw.ppjwa.cn

[R58] 下载文件
来源：http://mws.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wjy.ppjwa.cn

[R59] 发 POST JSON
来源：http://dlb.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uys.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://uca.ppjwa.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ljy.fktsv.cn

[R61] 磁盘占用
来源：http://rhn.meibo888.top

df -h;  du -sh *
来源：http://vqh.shzxlz.cn

[R62] 找最占空间的文件
来源：http://sme.tanke756.top

du -ah . | sort -rh | head -10
来源：http://mvp.yanxiufei.cn

[R63] 内存与进程
来源：http://fdr.haohaochexian.top

free -h;  ps aux | grep nginx
来源：http://wmj.yonumen.top

[R64] 结束进程
来源：http://mrf.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://kth.zycfv.cn

[R65] 查看端口占用
来源：http://rhi.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xto.birdmap.top

[R66] 定时任务
来源：http://hgp.dashuyun.cn

crontab -e;  crontab -l
来源：http://pma.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://zzw.ydjk.org.cn

openssl rand -hex 16
来源：http://wfq.svipenyu.cn

[R68] 计算文件校验值
来源：http://ovd.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://orb.mhx1999.top

[R69] 生成随机密码
来源：http://qka.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://fvw.daria6918.cn

[R70] 时间戳与互转
来源：http://tlm.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://zlt.c1oappe.top

[R71] 日期格式化
来源：http://vah.mhx1999.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bnt.c1oappe.top

[R72] 等待端口就绪
来源：http://izz.shuidangran.top

until nc -z localhost 3306; do sleep 1; done
来源：http://irn.jianghu66.top

[R73] 分割大日志
来源：http://vbl.xinyue.icu

split -l 1000 big.log part_
来源：http://mzw.jinqigfzy.top

[R74] 批量重命名
来源：http://dsq.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wny.guannengcc.top

[R75] 导出环境变量
来源：http://zmj.zhijiandao.cn

export PATH="$HOME/bin:$PATH"
来源：http://muj.hfpthk.cn

[R76] 使用临时文件
来源：http://faa.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ejm.jinqigufen.top

[R77] 读取用户输入
来源：http://fzz.aibaodan.cn

read -rp "请输入: " ans
来源：http://pap.yueranfly.top

[R78] 交互式菜单
来源：http://oto.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bfc.yuanzhike.top

[R79] 解析命令行选项
来源：http://szh.hysaishi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://old.sweek.top

[R80] 查看脚本执行耗时
来源：http://xxr.fzhhl.top

time ./run.sh
来源：http://vmn.hnqzz.top

================================================================================
来源：http://szg.meibo888.top

S. C / C++ 专题
来源：http://spn.wangshuangyany.cn

================================================================================
来源：http://kdy.wangdashe.top

[S01] C：Hello World
来源：http://atw.jiagoushi.top

#include <stdio.h>
来源：http://chm.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jse.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://ika.zhixingplan.top

int a = 10; printf("%d\n", a);
来源：http://uca.guowangkeji.top

[S03] C：读入整数
来源：http://ney.aibaodan.cn

int x; scanf("%d", &x);
来源：http://njb.hywenlv.cn

[S04] C：字符串复制
来源：http://udv.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wla.shzxlz.cn

[S05] C：字符串长度
来源：http://bkv.uphjek.com

strlen(s)
来源：http://yqq.ppjwa.cn

[S06] C：字符串比较
来源：http://hbr.yanxiufei.cn

strcmp(a, b) == 0
来源：http://fdf.ctjpmb.com

[S07] C：数组遍历求和
来源：http://tve.jyoumei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wha.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://yen.zycfv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://leh.jinqigufen.top

[S09] C：结构体定义与初始化
来源：http://yct.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tmx.zdqjudy.top

[S10] C：指针与解引用
来源：http://juz.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://ldk.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://anc.birdmap.top

FILE *f = fopen("a.txt", "r");
来源：http://gqk.yj20258.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yri.ydzc1.top

fclose(f);
来源：http://yle.yvedp.cn

[S12] C：写文件
来源：http://vxo.hammf.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gcn.wangdashe.top

[S13] C：宏定义
来源：http://ltv.redwolf501.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ogu.bjfxy.top

[S14] C：枚举
来源：http://yvv.hnxiangtu.top


<!-- 参考信息 -->