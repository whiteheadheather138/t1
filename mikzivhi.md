代发 wailian999

[Q48] CTE 公用表表达式
来源：http://sbh.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ixu.ydzc1.top

SELECT * FROM t WHERE c > 5;
来源：http://ouw.bbcook.cn

[Q49] 更新单行
来源：http://aml.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://syh.xziqi.cn

[Q50] 批量更新
来源：http://eyg.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://efp.sjlbkw.cn

[Q51] 用子查询更新
来源：http://rvg.ywan-chungtsiang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rqx.0kj1m.cn

[Q52] 删除指定行
来源：http://nga.andypj.xyz

DELETE FROM users WHERE id = 10;
来源：http://qgo.svipenyu.cn

[Q53] 按条件删除
来源：http://lfg.dashuyun.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uss.gotoacloud.top

[Q54] 清空表
来源：http://fmo.nwbrower.top

TRUNCATE TABLE logs;
来源：http://jdz.iojbl.cn

[Q55] 排名（并列占位）
来源：http://lpy.0kj1m.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://anc.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://ghk.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yjp.ybcxt.top

[Q57] 行号
来源：http://ppb.zhongyouzk.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gbh.quarkkingdee.top

[Q58] 累计求和
来源：http://jyb.hesvh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ypb.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://yon.sufxvd.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zwl.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://uwl.9152youxi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ife.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lgz.jqgfzy.top

[Q61] 移动平均
来源：http://lse.jianghu66.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rig.yvedp.cn

[Q62] 分组占比
来源：http://iob.zhijiandao.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dek.fehbvm.com

[Q63] 开启事务
来源：http://dea.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fpc.nwbrower.top

[Q64] 提交事务
来源：http://ahq.sweek.top

COMMIT;
来源：http://uig.fanxiaobao.xyz

[Q65] 回滚事务
来源：http://vhr.wangdashe.top

ROLLBACK;
来源：http://shh.hcnkem.com

[Q66] 行锁查询
来源：http://wln.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://piv.guannengcc.top

[Q67] 设置隔离级别
来源：http://xho.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zul.hnqzz.top

[Q68] 保存点
来源：http://dpn.yonumen.top

SAVEPOINT sp1;
来源：http://fqe.haohaochexian.top

ROLLBACK TO sp1;
来源：http://evj.daria6918.cn

[Q69] 查看执行计划
来源：http://heq.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wkx.wangshuangyany.cn

[Q70] 更新统计信息
来源：http://yfi.ybcxt.top

ANALYZE TABLE users;
来源：http://xvz.gogol.net.cn

[Q71] 查看建表语句
来源：http://ioj.chenjidiqi.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qgt.daria6918.cn

[Q72] 查看索引
来源：http://syj.hysaishi.cn

SHOW INDEX FROM users;
来源：http://njr.sweek.top

[Q73] 查看表状态
来源：http://mlm.xziqi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ped.hywenlv.cn

[Q74] 强制使用索引
来源：http://cnc.yuanzhike.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lsp.jinqigufen.top

[Q75] 日期格式化
来源：http://fxg.xylfe.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://alg.yj20258888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fqd.yuxming.cn

[Q76] 按天统计
来源：http://fxx.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cit.jinyuanbaomall.cn

[Q77] 时间加减
来源：http://qlz.zhijiandao.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nsk.xuanzx.com

[Q78] 当前时间
来源：http://nni.ydjk.org.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lzc.havefunace.top

[Q79] 字符串拼接
来源：http://mqe.dianchejie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uey.yongpay.top

[Q80] 字符串截取
来源：http://afw.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mto.shuidangran.top

[Q81] 字符串替换
来源：http://bid.guowangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uur.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://oyf.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wpw.mhx1999.top

[Q83] 大小写转换
来源：http://kvz.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jvt.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://clj.cucudq.cn

SELECT TRIM(name) FROM users;
来源：http://wkw.yonumen.top

[Q85] 数值取整
来源：http://vom.shangyingyoupin.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://evi.hammf.cn

[Q86] 读取 JSON 字段
来源：http://lrh.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gvg.hnqzz.top

[Q87] JSON 字段做条件
来源：http://gva.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bbn.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://ien.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ezn.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://boo.daxiang520.top

[Q89] 判断表是否存在
来源：http://cby.yj202588.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kmm.dashuyun.cn

[Q90] 生成序号列
来源：http://nek.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ttk.iojbl.cn

================================================================================
来源：http://gkf.bbcook.cn

R. Bash 专题
来源：http://tre.jqgufenzy.top

================================================================================
来源：http://kkm.9152youxi.cn

[R01] shebang 与严格模式
来源：http://qbt.zhongyouzk.top

#!/usr/bin/env bash
来源：http://vgm.jinghuilouyu.cn

set -euo pipefail
来源：http://xjg.gotoacloud.top

[R02] 变量赋值与使用
来源：http://ilf.tarul.cn

name="Tom"; echo "$name"
来源：http://bim.yuanzhike.top

[R03] 只读变量
来源：http://gzy.gaohongyu789.top

readonly PI=3.14
来源：http://vjj.meibo888.top

[R04] 位置参数
来源：http://pxh.316326.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oqj.daria6918.cn

[R05] 参数默认值
来源：http://tti.yangfankeji.com

name="${1:-default}"
来源：http://vka.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://ucz.gaohongyu789.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://skw.xuanzx.com

[R07] if 判断文件
来源：http://nne.daxiang520.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mbs.zhengqikj.top

[R08] 数值比较
来源：http://pfk.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zkm.guowangkeji.top

[R09] 字符串比较
来源：http://xew.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://brf.52xcode.cn

[R10] 正则匹配
来源：http://tug.havefunace.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nvv.daxiang520.top

[R11] case 多分支
来源：http://yvv.vehdjk.com

case "$1" in
来源：http://qxx.sweek.top

start) echo "启动" ;;
来源：http://bce.nanxinkj.top

stop)  echo "停止" ;;
来源：http://jen.sufxvd.cn

*)     echo "未知命令" ;;
来源：http://ogc.xuanzx.com

esac
来源：http://qrh.shanyushiyangkeji.top

[R12] for 遍历文件
来源：http://xle.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://ifg.chenlongwang.top

[R13] for 计数循环
来源：http://zfs.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://dtd.gotoacloud.top

[R14] C 风格 for
来源：http://rku.chenzaomai.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zfi.gotoacloud.top

[R15] while 逐行读文件
来源：http://jhl.0kj1m.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mwu.shuidangran.top

[R16] until 等待条件
来源：http://gau.dianchejie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eur.mhx1999.top

[R17] 数组定义与取值
来源：http://rhb.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nxb.haohaochexian.top

[R18] 遍历数组
来源：http://jya.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bar.fanxiaobao.xyz

[R19] 数组长度
来源：http://kak.smart0.xyz

echo "${#arr[@]}"
来源：http://bfe.yj20258.top

[R20] 关联数组（字典）
来源：http://oli.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rup.nanxuanxn.top

[R21] 字符串长度
来源：http://arc.nanxinkj.top

echo "${#s}"
来源：http://nyy.ivvv.top

[R22] 截取子串
来源：http://rzt.ybcxt.top

echo "${s:0:5}"
来源：http://zrk.yanxiufei.cn

[R23] 字符串替换
来源：http://tox.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ilx.zhengqikj.top

[R24] 大小写转换
来源：http://sdx.jqgfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://wmq.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://lil.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://qjo.kuanghao11.cn

[R26] 命令替换
来源：http://jzj.ivvv.top

now=$(date +%F); echo "$now"
来源：http://tiq.jlsjyb.cn

[R27] 算术展开
来源：http://tni.zhengqikj.top

echo $((1 + 2 * 3))
来源：http://pmr.uphjek.com

[R28] 浮点运算
来源：http://fvk.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://oig.ybcxt.top

[R29] 定义函数
来源：http://xay.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hnv.cqqwz.cn

[R30] 函数返回状态码
来源：http://wln.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://csq.daxiang520.top

[R31] 局部变量
来源：http://elh.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://mmu.redwolf501.top

[R32] 参数个数校验
来源：http://zab.sufxvd.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gxp.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://tbo.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ekp.gaohongyu789.top

[R34] 退出时清理
来源：http://cuu.nanxinkj.top

trap 'rm -f "$tmp"' EXIT
来源：http://vql.yvedp.cn

[R35] 后台执行并等待
来源：http://wvq.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://icv.zdqjudy.top

[R36] 并发执行多个任务
来源：http://ryn.meibo888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xxc.yueranfly.top

[R37] 把输出赋给变量
来源：http://foh.yanxiufei.cn

files=$(ls -1)
来源：http://pze.zhongyouzk.top

[R38] 管道串联
来源：http://zsu.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://vqq.shuidangran.top

[R39] 重定向标准输出与错误
来源：http://euc.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://wvt.yanxiufei.cn

[R40] 追加写日志
来源：http://xox.fengsongda.top

echo "log" >> out.log
来源：http://xlk.daxiang520.top

[R41] 丢弃输出
来源：http://atn.yfazqb.com

cmd >/dev/null 2>&1
来源：http://uua.kuanghao11.cn

[R42] 输入重定向
来源：http://kuw.redwolf501.top

wc -l < a.txt
来源：http://ndu.guannengcc.top

[R43] 按名字查找文件
来源：http://lcz.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://qvx.haohaochexian.top

[R44] 按修改时间查找
来源：http://rja.kuanghao11.cn

find . -mtime -7 -type f
来源：http://zyw.birdmap.top

[R45] 批量删除
来源：http://vxp.ydzc1.top

find . -name "*.tmp" -delete
来源：http://beo.jinghuilouyu.cn

[R46] 递归替换文件内容
来源：http://ovh.yanxiufei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zzm.jlsjyb.cn

[R47] sed 单行替换
来源：http://ycw.mhx1999.top

sed -i 's/foo/bar/g' a.txt
来源：http://tlx.cqqwz.cn

[R48] awk 取指定列
来源：http://axd.wangdashe.top

awk '{print $1, $3}' a.txt
来源：http://mmq.ehwqpu.com

[R49] awk 带条件
来源：http://huc.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kok.gotoacloud.top

[R50] awk 求和
来源：http://dvh.gaohongyu789.top

awk '{s += $2} END {print s}' a.txt
来源：http://ynr.ctjpmb.com

[R51] 排序去重取前几
来源：http://xhd.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://evd.hywenlv.cn

[R52] 统计行数
来源：http://qkh.nwbrower.top

wc -l a.txt
来源：http://hcx.epnwcf.com

[R53] 查看文件头与实时尾
来源：http://exe.fzhhl.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vhw.yvedp.cn

[R54] 比较两个文件
来源：http://ohb.sjlbkw.cn

diff a.txt b.txt
来源：http://ysv.guowangkeji.top

[R55] 压缩与解压
来源：http://jna.jinqigfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xkq.wangdashe.top

[R56] 远程拷贝
来源：http://mav.mhx1999.top

scp file user@host:/path/
来源：http://vde.hcnkem.com

[R57] 远程执行命令
来源：http://qla.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://rmz.pycfn.com

[R58] 下载文件
来源：http://gxf.yvedp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mng.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://rnh.yangfankeji.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ent.feifeiyinyue.top

[R60] 只看 HTTP 状态码
来源：http://evl.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://szt.ehwqpu.com

[R61] 磁盘占用
来源：http://aqo.mhx1999.top

df -h;  du -sh *
来源：http://zxm.mhx1999.top

[R62] 找最占空间的文件
来源：http://yik.smart0.xyz

du -ah . | sort -rh | head -10
来源：http://sxr.ivvv.top

[R63] 内存与进程
来源：http://guh.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://xcj.tarul.cn

[R64] 结束进程
来源：http://btp.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://rhw.chenlongwang.top

[R65] 查看端口占用
来源：http://ydb.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xdl.zdqjudy.top

[R66] 定时任务
来源：http://njw.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://ozc.daxiang520.top

[R67] 生成随机十六进制串
来源：http://qjw.ehwqpu.com

openssl rand -hex 16
来源：http://btc.jqgfzy.top

[R68] 计算文件校验值
来源：http://dyh.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dka.cheryme.top

[R69] 生成随机密码
来源：http://voa.shanyushiyangkeji.top

head -c 16 /dev/urandom | base64
来源：http://nfx.gaohongyu789.top

[R70] 时间戳与互转
来源：http://ovz.cashguo.top

date +%s;  date -d @1700000000
来源：http://liz.ivvv.top

[R71] 日期格式化
来源：http://nwd.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cur.zhongyouzk.top

[R72] 等待端口就绪
来源：http://bzk.mhx1999.top

until nc -z localhost 3306; do sleep 1; done
来源：http://eti.gzhubu.top

[R73] 分割大日志
来源：http://pgm.guowangkeji.top

split -l 1000 big.log part_
来源：http://uyy.c1oappe.top

[R74] 批量重命名
来源：http://fzb.xylfe.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jwe.fktsv.cn

[R75] 导出环境变量
来源：http://aaq.yj20258.top

export PATH="$HOME/bin:$PATH"
来源：http://cni.ybcxt.top

[R76] 使用临时文件
来源：http://llg.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tpp.hywenlv.cn

[R77] 读取用户输入
来源：http://lqq.xziqi.cn

read -rp "请输入: " ans
来源：http://pvt.ydzc1.top

[R78] 交互式菜单
来源：http://atj.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://qae.tarul.cn

[R79] 解析命令行选项
来源：http://fru.feifeiyinyue.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wwf.hnxiangtu.top

[R80] 查看脚本执行耗时
来源：http://qag.nanxuanxn.top

time ./run.sh
来源：http://ymu.hnxiangtu.top

================================================================================
来源：http://ats.xuetiantiany.cn

S. C / C++ 专题
来源：http://ygz.ctjpmb.com

================================================================================
来源：http://oxj.hnxiangtu.top

[S01] C：Hello World
来源：http://rcb.zhoulong.xyz

#include <stdio.h>
来源：http://gxq.vqdsnc.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xqd.zhengqikj.top

[S02] C：变量与格式化输出
来源：http://eku.ydzc1.top

int a = 10; printf("%d\n", a);
来源：http://ymx.xinyue.icu

[S03] C：读入整数
来源：http://peq.ctjpmb.com

int x; scanf("%d", &x);
来源：http://pdb.hesvh.cn

[S04] C：字符串复制
来源：http://hgg.aizwys.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gsy.sjlbkw.cn

[S05] C：字符串长度
来源：http://bcz.sweek.top

strlen(s)
来源：http://mhw.cdnleiting.top

[S06] C：字符串比较
来源：http://mfh.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://jqo.fengsongda.top

[S07] C：数组遍历求和
来源：http://nlf.ydzc1.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hqa.dashuyun.cn

[S08] C：动态内存分配与释放
来源：http://fsg.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qmy.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://moj.daxiang520.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://urf.hnxiangtu.top

[S10] C：指针与解引用
来源：http://lze.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://stg.tarul.cn

[S11] C：逐行读文件
来源：http://mdo.mhx1999.top

FILE *f = fopen("a.txt", "r");
来源：http://jlj.hnxiangtu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://utn.hywenlv.cn

fclose(f);
来源：http://snf.ppjwa.cn

[S12] C：写文件
来源：http://hpm.c1oappe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bkl.epnwcf.com

[S13] C：宏定义
来源：http://lzc.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://roz.hnqzz.top

[S14] C：枚举
来源：http://flj.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://hpn.ydzc1.top

[S15] C：类型转换
来源：http://yhc.hysaishi.cn

(double) a / b
来源：http://gdu.aibaodan.cn

[S16] C：位操作置位
来源：http://avn.shuidangran.top

x |= (1 << 3);
来源：http://vhp.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://wvb.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tsf.tian-w.cn

[S18] C：命令行参数
来源：http://ftg.xuanzx.com


<!-- 参考信息 -->