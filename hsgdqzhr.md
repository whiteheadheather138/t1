代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uug.zhixingplan.top

[Q50] 批量更新
来源：http://rwj.iojbl.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://plm.bbcook.cn

[Q51] 用子查询更新
来源：http://nfj.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lob.xuetiantiany.cn

[Q52] 删除指定行
来源：http://wwz.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://wlv.hfpthk.cn

[Q53] 按条件删除
来源：http://lja.aizwys.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gbn.hcnkem.com

[Q54] 清空表
来源：http://tmf.316326.xyz

TRUNCATE TABLE logs;
来源：http://bfj.hnqzz.top

[Q55] 排名（并列占位）
来源：http://udz.daxiang520.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kdi.smart0.xyz

[Q56] 密集排名（并列不占位）
来源：http://ohs.guowangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dir.cdnleiting.top

[Q57] 行号
来源：http://jmp.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tno.feifeiyinyue.top

[Q58] 累计求和
来源：http://ydq.zdbjq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gjj.sxryk.cn

[Q59] 分组内累计
来源：http://pmo.jqgufenzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ckh.aizwys.cn

[Q60] 取上一行 / 下一行
来源：http://ehx.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cqk.yangfankeji.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ioi.vqdsnc.cn

[Q61] 移动平均
来源：http://ytd.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jcv.ehwqpu.com

[Q62] 分组占比
来源：http://ikn.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nxo.gotoacloud.top

[Q63] 开启事务
来源：http://dys.hfpthk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lur.cheryme.top

[Q64] 提交事务
来源：http://xse.zhoulong.xyz

COMMIT;
来源：http://whi.guannengcc.top

[Q65] 回滚事务
来源：http://alx.aibaodan.cn

ROLLBACK;
来源：http://yem.zdbjq.cn

[Q66] 行锁查询
来源：http://xix.andypj.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nce.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://kza.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lky.daxiang520.top

[Q68] 保存点
来源：http://gpp.zdbjq.cn

SAVEPOINT sp1;
来源：http://ffq.hywenlv.cn

ROLLBACK TO sp1;
来源：http://uhn.ydzc1.top

[Q69] 查看执行计划
来源：http://qxo.shzxlz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ykx.shuidangran.top

[Q70] 更新统计信息
来源：http://mzs.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://cvf.fzhhl.top

[Q71] 查看建表语句
来源：http://jxd.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vgq.nanxinkj.top

[Q72] 查看索引
来源：http://juz.dianchejie.cn

SHOW INDEX FROM users;
来源：http://sal.uphjek.com

[Q73] 查看表状态
来源：http://hxj.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qby.zhaomingkeji.xyz

[Q74] 强制使用索引
来源：http://xir.gaohongyu789.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nsm.yueranfly.top

[Q75] 日期格式化
来源：http://qmw.guannengcc.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lhg.fanxiaobao.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cws.yangfankeji.com

[Q76] 按天统计
来源：http://vgd.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mjd.xuetiantiany.cn

[Q77] 时间加减
来源：http://fcx.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uyb.316326.xyz

[Q78] 当前时间
来源：http://mfx.nanxuanxn.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rrk.smart0.xyz

[Q79] 字符串拼接
来源：http://yge.shuidangran.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xtx.fengsongda.top

[Q80] 字符串截取
来源：http://waz.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://azw.yvedp.cn

[Q81] 字符串替换
来源：http://xsy.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zpb.birdmap.top

[Q82] 字符长度与字节长度
来源：http://xsu.52xcode.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ivn.vehdjk.com

[Q83] 大小写转换
来源：http://aqp.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ntl.tian-w.cn

[Q84] 去除首尾空格
来源：http://sgt.shuidangran.top

SELECT TRIM(name) FROM users;
来源：http://ueh.hammf.cn

[Q85] 数值取整
来源：http://gld.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fhd.haohaochexian.top

[Q86] 读取 JSON 字段
来源：http://xsu.daxiang520.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bwv.mhx1999.top

[Q87] JSON 字段做条件
来源：http://rih.chenjidiqi.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kon.tian-w.cn

[Q88] 行转列（条件聚合）
来源：http://uzy.jinghuilouyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gdb.shzxlz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kyw.hnxiangtu.top

[Q89] 判断表是否存在
来源：http://bun.fengsongda.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://har.0kj1m.cn

[Q90] 生成序号列
来源：http://oub.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qis.svipenyu.cn

================================================================================
来源：http://qqj.ctjpmb.com

R. Bash 专题
来源：http://bqz.hysaishi.cn

================================================================================
来源：http://vma.hnqzz.top

[R01] shebang 与严格模式
来源：http://dix.fzhhl.top

#!/usr/bin/env bash
来源：http://lfz.vqdsnc.cn

set -euo pipefail
来源：http://zyu.nanxuanxn.top

[R02] 变量赋值与使用
来源：http://hmi.bjfxy.top

name="Tom"; echo "$name"
来源：http://pca.shuidangran.top

[R03] 只读变量
来源：http://kgg.jinghuilouyu.cn

readonly PI=3.14
来源：http://isu.ppjwa.cn

[R04] 位置参数
来源：http://vzw.chenzaomai.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ocf.fehbvm.com

[R05] 参数默认值
来源：http://etw.316326.xyz

name="${1:-default}"
来源：http://ajs.yangfankeji.com

[R06] 判断命令是否存在
来源：http://icj.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://axt.fanxiaobao.xyz

[R07] if 判断文件
来源：http://rpf.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ull.tarul.cn

[R08] 数值比较
来源：http://jxg.yvedp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hqr.zhengqikj.top

[R09] 字符串比较
来源：http://cex.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sln.52xcode.cn

[R10] 正则匹配
来源：http://eng.daria6918.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ekd.birdmap.top

[R11] case 多分支
来源：http://awf.zycfv.cn

case "$1" in
来源：http://ljk.andypj.xyz

start) echo "启动" ;;
来源：http://exl.cucudq.cn

stop)  echo "停止" ;;
来源：http://wtl.shuidangran.top

*)     echo "未知命令" ;;
来源：http://qxr.nwbrower.top

esac
来源：http://bwu.hammf.cn

[R12] for 遍历文件
来源：http://upk.xingfuxueyuan.xyz

for f in *.txt; do echo "$f"; done
来源：http://ipl.jqgfzy.top

[R13] for 计数循环
来源：http://rsc.jqgfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://nqa.havefunace.top

[R14] C 风格 for
来源：http://qzc.birdmap.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sqh.tian-w.cn

[R15] while 逐行读文件
来源：http://jko.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yzu.xuetiantiany.cn

[R16] until 等待条件
来源：http://cdt.yj20258888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://otu.uphjek.com

[R17] 数组定义与取值
来源：http://par.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://dnb.nwbrower.top

[R18] 遍历数组
来源：http://ayx.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wep.redwolf501.top

[R19] 数组长度
来源：http://twg.tian-w.cn

echo "${#arr[@]}"
来源：http://bnk.xinyue.icu

[R20] 关联数组（字典）
来源：http://ksb.yuxming.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wpb.uphjek.com

[R21] 字符串长度
来源：http://mru.wangdashe.top

echo "${#s}"
来源：http://ocs.epnwcf.com

[R22] 截取子串
来源：http://trg.xuetiantiany.cn

echo "${s:0:5}"
来源：http://ypq.shangyingyoupin.top

[R23] 字符串替换
来源：http://oyv.hcnkem.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rhg.bbcook.cn

[R24] 大小写转换
来源：http://rum.yueranfly.top

echo "${s^^}"; echo "${s,,}"
来源：http://iqg.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://cba.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://etb.jinqigufen.top

[R26] 命令替换
来源：http://luc.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://dnp.ydzc1.top

[R27] 算术展开
来源：http://lfz.xziqi.cn

echo $((1 + 2 * 3))
来源：http://zst.yangfankeji.com

[R28] 浮点运算
来源：http://krc.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://asr.ybcxt.top

[R29] 定义函数
来源：http://pyp.mhx1999.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jec.pycfn.com

[R30] 函数返回状态码
来源：http://xqh.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://jbq.hfpthk.cn

[R31] 局部变量
来源：http://ewl.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://dtu.haohaochexian.top

[R32] 参数个数校验
来源：http://ovp.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oca.yonumen.top

[R33] 捕获错误并提示行号
来源：http://yax.nanxuanxn.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yym.tian-w.cn

[R34] 退出时清理
来源：http://kch.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://voa.quarkkingdee.top

[R35] 后台执行并等待
来源：http://eqe.shanyushiyangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ftr.smart0.xyz

[R36] 并发执行多个任务
来源：http://xor.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pdl.shangyingyoupin.top

[R37] 把输出赋给变量
来源：http://qbu.xuetiantiany.cn

files=$(ls -1)
来源：http://qql.ybcxt.top

[R38] 管道串联
来源：http://xie.sufxvd.cn

cat a.txt | grep -i error | wc -l
来源：http://fmg.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://ymb.cdnleiting.top

cmd > out.log 2>&1
来源：http://bjd.meibo888.top

[R40] 追加写日志
来源：http://gbq.sxryk.cn

echo "log" >> out.log
来源：http://ktl.hammf.cn

[R41] 丢弃输出
来源：http://wkb.tarul.cn

cmd >/dev/null 2>&1
来源：http://xhd.zycfv.cn

[R42] 输入重定向
来源：http://edi.zhixingplan.top

wc -l < a.txt
来源：http://ydg.smart0.xyz

[R43] 按名字查找文件
来源：http://llz.sxryk.cn

find . -name "*.log" -type f
来源：http://krr.gotoacloud.top

[R44] 按修改时间查找
来源：http://otf.ctjpmb.com

find . -mtime -7 -type f
来源：http://kax.ybcxt.top

[R45] 批量删除
来源：http://ymu.vehdjk.com

find . -name "*.tmp" -delete
来源：http://gzs.ybcxt.top

[R46] 递归替换文件内容
来源：http://pqy.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wod.xinyue.icu

[R47] sed 单行替换
来源：http://nme.zhongyouzk.top

sed -i 's/foo/bar/g' a.txt
来源：http://znp.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://hks.sxryk.cn

awk '{print $1, $3}' a.txt
来源：http://mkl.fzhhl.top

[R49] awk 带条件
来源：http://sln.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ted.tianlin.xyz

[R50] awk 求和
来源：http://mxb.havefunace.top

awk '{s += $2} END {print s}' a.txt
来源：http://cqi.ybcxt.top

[R51] 排序去重取前几
来源：http://nak.smart0.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://lkd.jinqigufen.top

[R52] 统计行数
来源：http://uwv.jianghu66.top

wc -l a.txt
来源：http://gmi.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://itj.c1oappe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ybu.pengpengdd.cyou

[R54] 比较两个文件
来源：http://pbj.gotoacloud.top

diff a.txt b.txt
来源：http://jkv.wangshuangyany.cn

[R55] 压缩与解压
来源：http://ixw.guannengcc.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fag.haohaochexian.top

[R56] 远程拷贝
来源：http://ked.zdqjudy.top

scp file user@host:/path/
来源：http://uig.xylfe.cn

[R57] 远程执行命令
来源：http://znt.yj20258888.top

ssh user@host 'uptime'
来源：http://ubc.zdqjudy.top

[R58] 下载文件
来源：http://gjq.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rfc.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://qzd.sjlbkw.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://akg.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://ikg.daxiang520.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://otz.fehbvm.com

[R61] 磁盘占用
来源：http://rpl.hcnkem.com

df -h;  du -sh *
来源：http://tho.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://kcv.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://dmm.yuxming.cn

[R63] 内存与进程
来源：http://uwd.hnqzz.top

free -h;  ps aux | grep nginx
来源：http://hex.yuxming.cn

[R64] 结束进程
来源：http://esa.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://ayt.quarkkingdee.top

[R65] 查看端口占用
来源：http://fkb.zhiwuduotai.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dyv.zdbjq.cn

[R66] 定时任务
来源：http://jpd.yanxiufei.cn

crontab -e;  crontab -l
来源：http://mpk.yvedp.cn

[R67] 生成随机十六进制串
来源：http://brz.redwolf501.top

openssl rand -hex 16
来源：http://btu.snrcjt.cn

[R68] 计算文件校验值
来源：http://evz.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zts.gaohongyu789.top

[R69] 生成随机密码
来源：http://lht.hesvh.cn

head -c 16 /dev/urandom | base64
来源：http://aqu.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://ozx.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://auv.sjlbkw.cn

[R71] 日期格式化
来源：http://oqq.mhx1999.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xbt.jinqigufen.top

[R72] 等待端口就绪
来源：http://yua.pengpengdd.cyou

until nc -z localhost 3306; do sleep 1; done
来源：http://ply.zdbjq.cn

[R73] 分割大日志
来源：http://svs.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://isx.feifeiyinyue.top

[R74] 批量重命名
来源：http://qly.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kta.316326.xyz

[R75] 导出环境变量
来源：http://ttt.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://rfr.dianchejie.cn

[R76] 使用临时文件
来源：http://cpx.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iut.cqqwz.cn

[R77] 读取用户输入
来源：http://ktx.nwbrower.top

read -rp "请输入: " ans
来源：http://yjj.xuetiantiany.cn

[R78] 交互式菜单
来源：http://qvx.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vha.wangdashe.top

[R79] 解析命令行选项
来源：http://zyu.aizwys.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ggy.pengpengdd.cyou

[R80] 查看脚本执行耗时
来源：http://loa.shzxlz.cn

time ./run.sh
来源：http://lng.kuanghao11.cn

================================================================================
来源：http://ojs.yongpay.top

S. C / C++ 专题
来源：http://psn.kuanghao11.cn

================================================================================
来源：http://hbm.gzhubu.top

[S01] C：Hello World
来源：http://sqx.ydzc1.top

#include <stdio.h>
来源：http://oeh.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kyn.316326.xyz

[S02] C：变量与格式化输出
来源：http://egq.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://iei.fehbvm.com

[S03] C：读入整数
来源：http://pep.yj202588.top

int x; scanf("%d", &x);
来源：http://crs.sysykeji.top

[S04] C：字符串复制
来源：http://vse.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ina.yongpay.top

[S05] C：字符串长度
来源：http://duw.mhx1999.top

strlen(s)
来源：http://ahw.yuxming.cn

[S06] C：字符串比较
来源：http://mkm.chenzaomai.com

strcmp(a, b) == 0
来源：http://zvb.zycfv.cn

[S07] C：数组遍历求和
来源：http://ohf.pengpengdd.cyou

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fia.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://uht.pengpengdd.cyou

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jhw.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://wyc.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://acd.hesvh.cn

[S10] C：指针与解引用
来源：http://jvf.316326.xyz

int *p = &a;  *p = 5;
来源：http://gvq.jlsjyb.cn

[S11] C：逐行读文件
来源：http://fhz.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://vtd.zhongyouzk.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://oup.shanyushiyangtech.top

fclose(f);
来源：http://rbl.zhixingplan.top

[S12] C：写文件
来源：http://gqn.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ihp.pycfn.com

[S13] C：宏定义
来源：http://tvj.daxiang520.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nqp.cheryme.top

[S14] C：枚举
来源：http://oub.meibo888.top

enum Color { RED, GREEN, BLUE };
来源：http://rkb.gotoacloud.top

[S15] C：类型转换
来源：http://sze.dashuyun.cn

(double) a / b
来源：http://myg.yj20258888.top

[S16] C：位操作置位
来源：http://rab.cucudq.cn

x |= (1 << 3);
来源：http://wbe.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://gdb.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rcv.xziqi.cn

[S18] C：命令行参数
来源：http://ibi.hysaishi.cn

int main(int argc, char **argv)
来源：http://use.ppjwa.cn

[S19] C：快速排序
来源：http://zoe.9152youxi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pmp.hywenlv.cn

[S20] C：二分查找
来源：http://lcf.yj20258.top


<!-- 参考信息 -->