代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://mcd.mhx1999.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cnh.jqgufenzy.top

[Q47] 与平均值比较
来源：http://tqs.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ger.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://iid.daxiang520.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zjy.vqdsnc.cn

SELECT * FROM t WHERE c > 5;
来源：http://gir.hysaishi.cn

[Q49] 更新单行
来源：http://zsh.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bjb.quarkkingdee.top

[Q50] 批量更新
来源：http://nnz.guannengcc.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://owg.fehbvm.com

[Q51] 用子查询更新
来源：http://dti.sufxvd.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ucg.tianlin.xyz

[Q52] 删除指定行
来源：http://vvt.cashguo.top

DELETE FROM users WHERE id = 10;
来源：http://gcb.jlsjyb.cn

[Q53] 按条件删除
来源：http://str.fktsv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tli.xuanzx.com

[Q54] 清空表
来源：http://uuj.bbcook.cn

TRUNCATE TABLE logs;
来源：http://zce.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://dlz.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ugz.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://kyv.ppjwa.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://brc.aizwys.cn

[Q57] 行号
来源：http://gcr.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tmf.meibo888.top

[Q58] 累计求和
来源：http://mqg.316326.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://euz.cucudq.cn

[Q59] 分组内累计
来源：http://yvs.gaohongyu789.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kdb.yonumen.top

[Q60] 取上一行 / 下一行
来源：http://ebj.ehwqpu.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xyc.guannengcc.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://alr.nwbrower.top

[Q61] 移动平均
来源：http://tbd.jqgufenzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mlp.chenzaomai.com

[Q62] 分组占比
来源：http://uuc.ywan-chungtsiang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qnj.nanxuanxn.top

[Q63] 开启事务
来源：http://eoi.sysykeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vle.mhx1999.top

[Q64] 提交事务
来源：http://dil.xuanzx.com

COMMIT;
来源：http://emq.andypj.xyz

[Q65] 回滚事务
来源：http://fxz.uphjek.com

ROLLBACK;
来源：http://fwe.chenzaomai.com

[Q66] 行锁查询
来源：http://xqv.gotoacloud.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hhk.gogol.net.cn

[Q67] 设置隔离级别
来源：http://fci.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ucq.cashguo.top

[Q68] 保存点
来源：http://mft.ctjpmb.com

SAVEPOINT sp1;
来源：http://rgv.yj20258.top

ROLLBACK TO sp1;
来源：http://dar.sjlbkw.cn

[Q69] 查看执行计划
来源：http://kuy.jinghuilouyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rfl.ywan-chungtsiang.top

[Q70] 更新统计信息
来源：http://nth.shzxlz.cn

ANALYZE TABLE users;
来源：http://umm.fktsv.cn

[Q71] 查看建表语句
来源：http://afi.svipenyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pcp.ydzc1.top

[Q72] 查看索引
来源：http://fjs.vehdjk.com

SHOW INDEX FROM users;
来源：http://uck.shanyushiyangkeji.top

[Q73] 查看表状态
来源：http://bes.hnxiangtu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jkq.cashguo.top

[Q74] 强制使用索引
来源：http://gtb.xuetiantiany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://csb.feifeiyinyue.top

[Q75] 日期格式化
来源：http://dyz.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kof.sysykeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yma.ybcxt.top

[Q76] 按天统计
来源：http://usa.fzhhl.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jcp.zhengqikj.top

[Q77] 时间加减
来源：http://yiu.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://syu.epnwcf.com

[Q78] 当前时间
来源：http://huu.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yta.yvedp.cn

[Q79] 字符串拼接
来源：http://zzd.zhijiandao.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iir.xingfuxueyuan.xyz

[Q80] 字符串截取
来源：http://tez.zhongyouzk.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nid.hesvh.cn

[Q81] 字符串替换
来源：http://mgn.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vmq.c1oappe.top

[Q82] 字符长度与字节长度
来源：http://clj.dianchejie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://otd.wangshuangyany.cn

[Q83] 大小写转换
来源：http://zto.zhoulong.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://odb.cdnleiting.top

[Q84] 去除首尾空格
来源：http://qtb.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://rdu.ctjpmb.com

[Q85] 数值取整
来源：http://fiq.gotoacloud.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mrq.haohaochexian.top

[Q86] 读取 JSON 字段
来源：http://gdy.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tgb.xuanzx.com

[Q87] JSON 字段做条件
来源：http://kit.bjfxy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tvt.epnwcf.com

[Q88] 行转列（条件聚合）
来源：http://uvn.yuxming.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qgj.jinqigfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pux.daxiang520.top

[Q89] 判断表是否存在
来源：http://vkf.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ake.fehbvm.com

[Q90] 生成序号列
来源：http://inp.ctjpmb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iff.quarkkingdee.top

================================================================================
来源：http://lai.hnqzz.top

R. Bash 专题
来源：http://zgs.gzhubu.top

================================================================================
来源：http://lhg.daxiang520.top

[R01] shebang 与严格模式
来源：http://gzg.gogol.net.cn

#!/usr/bin/env bash
来源：http://ddz.xziqi.cn

set -euo pipefail
来源：http://xty.jqgufenzy.top

[R02] 变量赋值与使用
来源：http://zme.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://zkm.cashguo.top

[R03] 只读变量
来源：http://sxz.yonumen.top

readonly PI=3.14
来源：http://goi.wangshuangyany.cn

[R04] 位置参数
来源：http://hjb.shanyushiyangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tld.yueranfly.top

[R05] 参数默认值
来源：http://xkg.haohaochexian.top

name="${1:-default}"
来源：http://aub.fzhhl.top

[R06] 判断命令是否存在
来源：http://apy.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ycn.shuidangran.top

[R07] if 判断文件
来源：http://mgs.hongshengwenyu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hov.xuetiantiany.cn

[R08] 数值比较
来源：http://ril.epnwcf.com

if (( a > b )); then echo "a 更大"; fi
来源：http://kyh.fehbvm.com

[R09] 字符串比较
来源：http://hbt.xingfuxueyuan.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sga.jinqigfzy.top

[R10] 正则匹配
来源：http://uqz.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://byw.sysykeji.top

[R11] case 多分支
来源：http://xli.xylfe.cn

case "$1" in
来源：http://fal.dashuyun.cn

start) echo "启动" ;;
来源：http://acm.ywan-chungtsiang.top

stop)  echo "停止" ;;
来源：http://dfr.sysykeji.top

*)     echo "未知命令" ;;
来源：http://jux.yangfankeji.com

esac
来源：http://dbs.jinqigufen.top

[R12] for 遍历文件
来源：http://ced.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://cmc.sjlbkw.cn

[R13] for 计数循环
来源：http://xuy.hnqzz.top

for i in {1..10}; do echo "$i"; done
来源：http://kes.yvedp.cn

[R14] C 风格 for
来源：http://cjo.hywenlv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uhb.yj20258.top

[R15] while 逐行读文件
来源：http://dzj.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gag.xuanzx.com

[R16] until 等待条件
来源：http://lls.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://til.nanxinkj.top

[R17] 数组定义与取值
来源：http://ked.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://fvz.cheryme.top

[R18] 遍历数组
来源：http://hfr.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uke.feifeiyinyue.top

[R19] 数组长度
来源：http://xae.jiagoushi.top

echo "${#arr[@]}"
来源：http://ntq.hcnkem.com

[R20] 关联数组（字典）
来源：http://rxc.kuanghao11.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aiu.yueranfly.top

[R21] 字符串长度
来源：http://orv.tarul.cn

echo "${#s}"
来源：http://azz.fengsongda.top

[R22] 截取子串
来源：http://euj.zycfv.cn

echo "${s:0:5}"
来源：http://zcq.0kj1m.cn

[R23] 字符串替换
来源：http://sic.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dsr.andypj.xyz

[R24] 大小写转换
来源：http://yzu.yanxiufei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://twa.uphjek.com

[R25] 去后缀 / 去前缀
来源：http://vxz.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://zth.tanke756.top

[R26] 命令替换
来源：http://qxe.yonumen.top

now=$(date +%F); echo "$now"
来源：http://zzd.xuetiantiany.cn

[R27] 算术展开
来源：http://klu.ywan-chungtsiang.top

echo $((1 + 2 * 3))
来源：http://yru.gzhubu.top

[R28] 浮点运算
来源：http://umd.smart0.xyz

echo "scale=2; 10/3" | bc
来源：http://kjx.ehwqpu.com

[R29] 定义函数
来源：http://toz.yongpay.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tkb.jinqigufen.top

[R30] 函数返回状态码
来源：http://ipw.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://fos.hnqzz.top

[R31] 局部变量
来源：http://mhy.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://twe.cucudq.cn

[R32] 参数个数校验
来源：http://voy.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://glh.cheryme.top

[R33] 捕获错误并提示行号
来源：http://lbe.jianghu66.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dcq.cqqwz.cn

[R34] 退出时清理
来源：http://eos.sufxvd.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ads.zhaomingkeji.xyz

[R35] 后台执行并等待
来源：http://acc.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vic.daria6918.cn

[R36] 并发执行多个任务
来源：http://qed.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ool.shanyushiyangkeji.top

[R37] 把输出赋给变量
来源：http://yuh.svipenyu.cn

files=$(ls -1)
来源：http://uev.jiagoushi.top

[R38] 管道串联
来源：http://mne.tianlin.xyz

cat a.txt | grep -i error | wc -l
来源：http://zwp.xingfuxueyuan.xyz

[R39] 重定向标准输出与错误
来源：http://ovo.52xcode.cn

cmd > out.log 2>&1
来源：http://ofq.52xcode.cn

[R40] 追加写日志
来源：http://vtk.chenlongwang.top

echo "log" >> out.log
来源：http://cbd.52xcode.cn

[R41] 丢弃输出
来源：http://cxw.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://syk.andypj.xyz

[R42] 输入重定向
来源：http://tsn.yvedp.cn

wc -l < a.txt
来源：http://luy.jqgufenzy.top

[R43] 按名字查找文件
来源：http://mgu.xuetiantiany.cn

find . -name "*.log" -type f
来源：http://jlq.zhoulong.xyz

[R44] 按修改时间查找
来源：http://pxn.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://rxe.fengsongda.top

[R45] 批量删除
来源：http://hib.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://adu.zhaomingkeji.xyz

[R46] 递归替换文件内容
来源：http://tid.zhijiandao.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yyv.fzhhl.top

[R47] sed 单行替换
来源：http://ssd.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://dzq.iojbl.cn

[R48] awk 取指定列
来源：http://obe.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://cyd.wangdashe.top

[R49] awk 带条件
来源：http://vlw.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iav.sxryk.cn

[R50] awk 求和
来源：http://wca.haohaochexian.top

awk '{s += $2} END {print s}' a.txt
来源：http://swb.daria6918.cn

[R51] 排序去重取前几
来源：http://ghe.shangyingyoupin.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bpf.cucudq.cn

[R52] 统计行数
来源：http://xgd.yj202588.top

wc -l a.txt
来源：http://bok.sjlbkw.cn

[R53] 查看文件头与实时尾
来源：http://gdh.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bdr.dianchejie.cn

[R54] 比较两个文件
来源：http://elu.zycfv.cn

diff a.txt b.txt
来源：http://vlb.uphjek.com

[R55] 压缩与解压
来源：http://jsn.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lsg.zdbjq.cn

[R56] 远程拷贝
来源：http://ikd.cdnleiting.top

scp file user@host:/path/
来源：http://yoj.zdqjudy.top

[R57] 远程执行命令
来源：http://pge.epnwcf.com

ssh user@host 'uptime'
来源：http://iux.daxiang520.top

[R58] 下载文件
来源：http://mdv.hysaishi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hxu.yangfankeji.com

[R59] 发 POST JSON
来源：http://luy.sweek.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lds.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://sin.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qzy.jianghu66.top

[R61] 磁盘占用
来源：http://run.yfazqb.com

df -h;  du -sh *
来源：http://izt.tanke756.top

[R62] 找最占空间的文件
来源：http://ivw.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://fwy.bjfxy.top

[R63] 内存与进程
来源：http://txo.hongshengwenyu.top

free -h;  ps aux | grep nginx
来源：http://sln.jiagoushi.top

[R64] 结束进程
来源：http://byd.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://zkx.nwbrower.top

[R65] 查看端口占用
来源：http://mxd.feifeiyinyue.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eem.nanxuanxn.top

[R66] 定时任务
来源：http://zpe.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://shl.dianchejie.cn

[R67] 生成随机十六进制串
来源：http://gxl.zhengqikj.top

openssl rand -hex 16
来源：http://lkg.zhiwuduotai.top

[R68] 计算文件校验值
来源：http://mwv.redwolf501.top

sha256sum a.txt;  md5sum a.txt
来源：http://ibc.zhixingplan.top

[R69] 生成随机密码
来源：http://plr.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://jjb.yonumen.top

[R70] 时间戳与互转
来源：http://uny.hcnkem.com

date +%s;  date -d @1700000000
来源：http://psq.jinqigufen.top

[R71] 日期格式化
来源：http://oji.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qid.hywenlv.cn

[R72] 等待端口就绪
来源：http://fxw.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rcp.fehbvm.com

[R73] 分割大日志
来源：http://ntx.bjfxy.top

split -l 1000 big.log part_
来源：http://ysh.nwbrower.top

[R74] 批量重命名
来源：http://iir.pycfn.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jng.sjlbkw.cn

[R75] 导出环境变量
来源：http://huc.shuidangran.top

export PATH="$HOME/bin:$PATH"
来源：http://ojf.jlsjyb.cn

[R76] 使用临时文件
来源：http://wmy.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ufb.tarul.cn

[R77] 读取用户输入
来源：http://ozf.xylfe.cn

read -rp "请输入: " ans
来源：http://evb.sufxvd.cn

[R78] 交互式菜单
来源：http://etm.smart0.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://mlk.jlsjyb.cn

[R79] 解析命令行选项
来源：http://nxj.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://czj.zycfv.cn

[R80] 查看脚本执行耗时
来源：http://xwy.feifeiyinyue.top

time ./run.sh
来源：http://dje.zhoulong.xyz

================================================================================
来源：http://ubr.fanxiaobao.xyz

S. C / C++ 专题
来源：http://qlr.svipenyu.cn

================================================================================
来源：http://tqe.yj20258888.top

[S01] C：Hello World
来源：http://mev.kuanghao11.cn

#include <stdio.h>
来源：http://jwe.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kqb.guowangkeji.top

[S02] C：变量与格式化输出
来源：http://jxx.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://txo.hesvh.cn

[S03] C：读入整数
来源：http://ehi.yongpay.top

int x; scanf("%d", &x);
来源：http://fkr.gotoacloud.top

[S04] C：字符串复制
来源：http://qrx.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ttr.zhoulong.xyz

[S05] C：字符串长度
来源：http://yry.nanxuanxn.top

strlen(s)
来源：http://vuv.hnqzz.top

[S06] C：字符串比较
来源：http://nal.meibo888.top

strcmp(a, b) == 0
来源：http://cex.ybcxt.top

[S07] C：数组遍历求和
来源：http://tto.sxryk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://esj.ivvv.top

[S08] C：动态内存分配与释放
来源：http://oys.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wtu.vehdjk.com

[S09] C：结构体定义与初始化
来源：http://kvr.hesvh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yij.0kj1m.cn

[S10] C：指针与解引用
来源：http://drp.316326.xyz

int *p = &a;  *p = 5;
来源：http://bss.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://srr.c1oappe.top

FILE *f = fopen("a.txt", "r");
来源：http://sjk.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://llm.c1oappe.top

fclose(f);
来源：http://sxv.cucudq.cn

[S12] C：写文件
来源：http://qhs.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kwh.zhiwuduotai.top

[S13] C：宏定义
来源：http://ajg.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fca.fengsongda.top

[S14] C：枚举
来源：http://zim.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://ipn.jlsjyb.cn

[S15] C：类型转换
来源：http://cqd.uphjek.com

(double) a / b
来源：http://tsi.ehwqpu.com

[S16] C：位操作置位
来源：http://sur.bbcook.cn


<!-- 参考信息 -->