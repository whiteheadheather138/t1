代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yvh.haohaochexian.top

[Q54] 清空表
来源：http://nrv.yfazqb.com

TRUNCATE TABLE logs;
来源：http://skb.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://woi.ivvv.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ojr.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://bwv.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oeo.yj20258.top

[Q57] 行号
来源：http://mqa.daxiang520.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://laz.zhongyouzk.top

[Q58] 累计求和
来源：http://xgx.nwbrower.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xtc.guannengcc.top

[Q59] 分组内累计
来源：http://ltg.zhengqikj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rjv.quarkkingdee.top

[Q60] 取上一行 / 下一行
来源：http://sic.xziqi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ica.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cno.guowangkeji.top

[Q61] 移动平均
来源：http://hsp.nwbrower.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ghn.yuxming.cn

[Q62] 分组占比
来源：http://gtq.epnwcf.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lsj.jqgufenzy.top

[Q63] 开启事务
来源：http://sht.jinghuilouyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ygo.cheryme.top

[Q64] 提交事务
来源：http://tcr.aibaodan.cn

COMMIT;
来源：http://kyl.yanxiufei.cn

[Q65] 回滚事务
来源：http://ulu.fzhhl.top

ROLLBACK;
来源：http://xis.ivvv.top

[Q66] 行锁查询
来源：http://vzx.yueranfly.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gjw.wangshuangyany.cn

[Q67] 设置隔离级别
来源：http://mdc.svipenyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ejp.feifeiyinyue.top

[Q68] 保存点
来源：http://xyx.zhijiandao.cn

SAVEPOINT sp1;
来源：http://dpo.sufxvd.cn

ROLLBACK TO sp1;
来源：http://qcr.guowangkeji.top

[Q69] 查看执行计划
来源：http://gsr.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nds.zycfv.cn

[Q70] 更新统计信息
来源：http://sao.zhixingplan.top

ANALYZE TABLE users;
来源：http://qqv.yfazqb.com

[Q71] 查看建表语句
来源：http://jum.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lgq.cheryme.top

[Q72] 查看索引
来源：http://ink.dianchejie.cn

SHOW INDEX FROM users;
来源：http://syf.hongshengwenyu.top

[Q73] 查看表状态
来源：http://ypx.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://opk.cdnleiting.top

[Q74] 强制使用索引
来源：http://leu.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eiy.yfazqb.com

[Q75] 日期格式化
来源：http://umh.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zyo.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ots.gaohongyu789.top

[Q76] 按天统计
来源：http://kvt.sxryk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://urg.xylfe.cn

[Q77] 时间加减
来源：http://bzr.tianlin.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zxq.bjfxy.top

[Q78] 当前时间
来源：http://dcp.zhaomingkeji.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ifa.ydjk.org.cn

[Q79] 字符串拼接
来源：http://bne.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iqu.xuanzx.com

[Q80] 字符串截取
来源：http://rbx.pycfn.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ekd.hywenlv.cn

[Q81] 字符串替换
来源：http://tki.gaohongyu789.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fwi.svipenyu.cn

[Q82] 字符长度与字节长度
来源：http://jnc.hnqzz.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ukl.nanxinkj.top

[Q83] 大小写转换
来源：http://odb.hnqzz.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qtx.dianchejie.cn

[Q84] 去除首尾空格
来源：http://wot.jinyuanbaomall.cn

SELECT TRIM(name) FROM users;
来源：http://wyj.jiagoushi.top

[Q85] 数值取整
来源：http://sog.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qjr.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://dit.yongpay.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oxj.zycfv.cn

[Q87] JSON 字段做条件
来源：http://oyt.nanxuanxn.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qpk.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://iwl.sufxvd.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kuk.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ivy.pycfn.com

[Q89] 判断表是否存在
来源：http://jjw.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zor.zhaomingkeji.xyz

[Q90] 生成序号列
来源：http://sgc.jqgufenzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://csz.shzxlz.cn

================================================================================
来源：http://qbs.tanke756.top

R. Bash 专题
来源：http://hwd.nanxinkj.top

================================================================================
来源：http://nzp.hysaishi.cn

[R01] shebang 与严格模式
来源：http://pye.hnxiangtu.top

#!/usr/bin/env bash
来源：http://rvk.yanxiufei.cn

set -euo pipefail
来源：http://nhd.yfazqb.com

[R02] 变量赋值与使用
来源：http://cor.mhx1999.top

name="Tom"; echo "$name"
来源：http://twt.ydjk.org.cn

[R03] 只读变量
来源：http://xor.chenlongwang.top

readonly PI=3.14
来源：http://rxa.cdnleiting.top

[R04] 位置参数
来源：http://cbs.zhixingplan.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tnw.tarul.cn

[R05] 参数默认值
来源：http://bvw.ivvv.top

name="${1:-default}"
来源：http://ypu.ybcxt.top

[R06] 判断命令是否存在
来源：http://byr.ywan-chungtsiang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iod.epnwcf.com

[R07] if 判断文件
来源：http://wcf.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yen.sjlbkw.cn

[R08] 数值比较
来源：http://dxi.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mqx.cdnleiting.top

[R09] 字符串比较
来源：http://rpr.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mwa.c1oappe.top

[R10] 正则匹配
来源：http://gat.daxiang520.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pyc.shanyushiyangtech.top

[R11] case 多分支
来源：http://jfh.smart0.xyz

case "$1" in
来源：http://tkd.jinqigfzy.top

start) echo "启动" ;;
来源：http://rcy.shanyushiyangtech.top

stop)  echo "停止" ;;
来源：http://kjk.zycfv.cn

*)     echo "未知命令" ;;
来源：http://igi.shangyingyoupin.top

esac
来源：http://trg.xuetiantiany.cn

[R12] for 遍历文件
来源：http://zdy.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://wyb.daxiang520.top

[R13] for 计数循环
来源：http://cxa.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://cip.yuxming.cn

[R14] C 风格 for
来源：http://pfv.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://egj.xuetiantiany.cn

[R15] while 逐行读文件
来源：http://rjt.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tyt.ehwqpu.com

[R16] until 等待条件
来源：http://lhv.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rgf.jiagoushi.top

[R17] 数组定义与取值
来源：http://ubi.nanxinkj.top

arr=(a b c); echo "${arr[0]}"
来源：http://xrw.dianchejie.cn

[R18] 遍历数组
来源：http://kde.svipenyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kzf.xziqi.cn

[R19] 数组长度
来源：http://etd.zhiwuduotai.top

echo "${#arr[@]}"
来源：http://gic.yongpay.top

[R20] 关联数组（字典）
来源：http://eqo.jinyuanbaomall.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jvr.guannengcc.top

[R21] 字符串长度
来源：http://xwc.xinyue.icu

echo "${#s}"
来源：http://lbo.sxryk.cn

[R22] 截取子串
来源：http://qfm.jqgufenzy.top

echo "${s:0:5}"
来源：http://aay.52xcode.cn

[R23] 字符串替换
来源：http://tof.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ykr.snrcjt.cn

[R24] 大小写转换
来源：http://buk.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://tir.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://ybg.daria6918.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qin.nanxinkj.top

[R26] 命令替换
来源：http://ybx.mhx1999.top

now=$(date +%F); echo "$now"
来源：http://zck.nanxuanxn.top

[R27] 算术展开
来源：http://mtl.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://hvt.xylfe.cn

[R28] 浮点运算
来源：http://viq.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://uvu.xingfuxueyuan.xyz

[R29] 定义函数
来源：http://vqt.aizwys.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://epf.zdbjq.cn

[R30] 函数返回状态码
来源：http://kch.sweek.top

f() { return 0; }; f || echo "失败了"
来源：http://dvz.jqgufenzy.top

[R31] 局部变量
来源：http://its.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://qnu.yuxming.cn

[R32] 参数个数校验
来源：http://uii.hysaishi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://crc.yfazqb.com

[R33] 捕获错误并提示行号
来源：http://nkm.jiagoushi.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://asd.uphjek.com

[R34] 退出时清理
来源：http://ewl.pengpengdd.cyou

trap 'rm -f "$tmp"' EXIT
来源：http://klw.bjfxy.top

[R35] 后台执行并等待
来源：http://amw.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vut.yuanzhike.top

[R36] 并发执行多个任务
来源：http://hta.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xlx.hesvh.cn

[R37] 把输出赋给变量
来源：http://fyd.yueranfly.top

files=$(ls -1)
来源：http://ldk.zdbjq.cn

[R38] 管道串联
来源：http://oqw.guannengcc.top

cat a.txt | grep -i error | wc -l
来源：http://gvr.dianchejie.cn

[R39] 重定向标准输出与错误
来源：http://ijp.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://tae.zhoulong.xyz

[R40] 追加写日志
来源：http://vls.sufxvd.cn

echo "log" >> out.log
来源：http://jyi.shuidangran.top

[R41] 丢弃输出
来源：http://lrq.tarul.cn

cmd >/dev/null 2>&1
来源：http://eqy.cqqwz.cn

[R42] 输入重定向
来源：http://ayl.iojbl.cn

wc -l < a.txt
来源：http://sin.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://dot.ctjpmb.com

find . -name "*.log" -type f
来源：http://nlr.c1oappe.top

[R44] 按修改时间查找
来源：http://pya.xuetiantiany.cn

find . -mtime -7 -type f
来源：http://upw.dianchejie.cn

[R45] 批量删除
来源：http://nrd.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://glq.epnwcf.com

[R46] 递归替换文件内容
来源：http://xvv.meibo888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hqs.zdbjq.cn

[R47] sed 单行替换
来源：http://elb.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://mdw.yongpay.top

[R48] awk 取指定列
来源：http://jvo.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://zll.zhoulong.xyz

[R49] awk 带条件
来源：http://vvx.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qkm.zhengqikj.top

[R50] awk 求和
来源：http://stb.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wma.meibo888.top

[R51] 排序去重取前几
来源：http://osr.wangshuangyany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kmb.wangshuangyany.cn

[R52] 统计行数
来源：http://pha.zhoulong.xyz

wc -l a.txt
来源：http://xyx.nwbrower.top

[R53] 查看文件头与实时尾
来源：http://cha.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sgw.aibaodan.cn

[R54] 比较两个文件
来源：http://rya.shzxlz.cn

diff a.txt b.txt
来源：http://ond.hysaishi.cn

[R55] 压缩与解压
来源：http://djo.bbcook.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tcz.yvedp.cn

[R56] 远程拷贝
来源：http://thl.bjfxy.top

scp file user@host:/path/
来源：http://erg.wangshuangyany.cn

[R57] 远程执行命令
来源：http://dju.haohaochexian.top

ssh user@host 'uptime'
来源：http://eyg.yangfankeji.com

[R58] 下载文件
来源：http://hng.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oer.hnxiangtu.top

[R59] 发 POST JSON
来源：http://qoj.hnxiangtu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qer.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://khw.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nrt.sweek.top

[R61] 磁盘占用
来源：http://typ.gaohongyu789.top

df -h;  du -sh *
来源：http://slq.cdnleiting.top

[R62] 找最占空间的文件
来源：http://gew.jyoumei.cn

du -ah . | sort -rh | head -10
来源：http://yzj.zycfv.cn

[R63] 内存与进程
来源：http://nwa.hnxiangtu.top

free -h;  ps aux | grep nginx
来源：http://jfy.redwolf501.top

[R64] 结束进程
来源：http://qzc.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://iqu.yanxiufei.cn

[R65] 查看端口占用
来源：http://jbp.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zcv.fengsongda.top

[R66] 定时任务
来源：http://cwl.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://gpe.yfazqb.com

[R67] 生成随机十六进制串
来源：http://rpz.ydzc1.top

openssl rand -hex 16
来源：http://ccm.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://wir.yj20258888.top

sha256sum a.txt;  md5sum a.txt
来源：http://glk.mhx1999.top

[R69] 生成随机密码
来源：http://zht.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://koc.zycfv.cn

[R70] 时间戳与互转
来源：http://szs.fehbvm.com

date +%s;  date -d @1700000000
来源：http://kep.316326.xyz

[R71] 日期格式化
来源：http://xvr.aibaodan.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wqb.zhengqikj.top

[R72] 等待端口就绪
来源：http://hbz.shanyushiyangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nvi.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://ort.vehdjk.com

split -l 1000 big.log part_
来源：http://bsr.epnwcf.com

[R74] 批量重命名
来源：http://omv.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ozc.aibaodan.cn

[R75] 导出环境变量
来源：http://cup.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://icq.cheryme.top

[R76] 使用临时文件
来源：http://xwc.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wvm.yonumen.top

[R77] 读取用户输入
来源：http://mjt.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://pfw.zhengqikj.top

[R78] 交互式菜单
来源：http://cmi.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iua.pycfn.com

[R79] 解析命令行选项
来源：http://wpm.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fol.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://uxz.xuetiantiany.cn

time ./run.sh
来源：http://lwj.andypj.xyz

================================================================================
来源：http://dkz.yj20258.top

S. C / C++ 专题
来源：http://aiy.birdmap.top

================================================================================
来源：http://wug.yuxming.cn

[S01] C：Hello World
来源：http://myd.kuanghao11.cn

#include <stdio.h>
来源：http://luq.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://mzj.ywan-chungtsiang.top

[S02] C：变量与格式化输出
来源：http://cpb.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://con.hysaishi.cn

[S03] C：读入整数
来源：http://bhg.shzxlz.cn

int x; scanf("%d", &x);
来源：http://drm.hongshengwenyu.top

[S04] C：字符串复制
来源：http://wmw.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mhq.xuanzx.com

[S05] C：字符串长度
来源：http://tuc.yuanzhike.top

strlen(s)
来源：http://tth.zdqjudy.top

[S06] C：字符串比较
来源：http://ixp.andypj.xyz

strcmp(a, b) == 0
来源：http://ykt.fengsongda.top

[S07] C：数组遍历求和
来源：http://apw.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eta.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://qhn.hesvh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vog.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://qzk.smart0.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://his.yanxiufei.cn

[S10] C：指针与解引用
来源：http://spz.chenzaomai.com

int *p = &a;  *p = 5;
来源：http://bhc.ydzc1.top

[S11] C：逐行读文件
来源：http://nnb.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "r");
来源：http://abx.zycfv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qwb.c1oappe.top

fclose(f);
来源：http://ina.aizwys.cn

[S12] C：写文件
来源：http://amz.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lux.uphjek.com

[S13] C：宏定义
来源：http://frh.wangdashe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vwb.jinqigfzy.top

[S14] C：枚举
来源：http://pew.fengsongda.top

enum Color { RED, GREEN, BLUE };
来源：http://gwt.xinyue.icu

[S15] C：类型转换
来源：http://slx.gotoacloud.top

(double) a / b
来源：http://zwi.wangshuangyany.cn

[S16] C：位操作置位
来源：http://ibz.andypj.xyz

x |= (1 << 3);
来源：http://rre.gzhubu.top

[S17] C：安全拼接字符串
来源：http://vld.dashuyun.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vzk.smart0.xyz

[S18] C：命令行参数
来源：http://gku.cqqwz.cn

int main(int argc, char **argv)
来源：http://qnk.shuidangran.top

[S19] C：快速排序
来源：http://mmt.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://mas.tian-w.cn

[S20] C：二分查找
来源：http://hpd.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mdf.ppjwa.cn

[S21] C：字符类别判断
来源：http://lsn.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gus.c1oappe.top

[S22] C：字符串转数字
来源：http://kgd.ywan-chungtsiang.top

atoi("42");  strtod("3.14", NULL);
来源：http://wrz.xuetiantiany.cn

[S23] C：随机数
来源：http://sau.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nyg.bjfxy.top

[S24] C：获取本地时间
来源：http://xzc.kuanghao11.cn


<!-- 参考信息 -->