代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vfo.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://ohj.aizwys.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pvi.tanke756.top

[Q57] 行号
来源：http://qsc.jqgufenzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hjp.sxryk.cn

[Q58] 累计求和
来源：http://orx.316326.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qna.haohaochexian.top

[Q59] 分组内累计
来源：http://jat.chenjidiqi.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sdl.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://elr.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qtn.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tug.snrcjt.cn

[Q61] 移动平均
来源：http://bpm.hongshengwenyu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ezr.meibo888.top

[Q62] 分组占比
来源：http://vqm.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tio.ybcxt.top

[Q63] 开启事务
来源：http://zwv.daria6918.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tlm.cashguo.top

[Q64] 提交事务
来源：http://gug.hywenlv.cn

COMMIT;
来源：http://pnn.daria6918.cn

[Q65] 回滚事务
来源：http://rvu.havefunace.top

ROLLBACK;
来源：http://auu.fzhhl.top

[Q66] 行锁查询
来源：http://iio.ehwqpu.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qvi.smart0.xyz

[Q67] 设置隔离级别
来源：http://phu.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pqu.guowangkeji.top

[Q68] 保存点
来源：http://vlb.sjlbkw.cn

SAVEPOINT sp1;
来源：http://yvx.shuidangran.top

ROLLBACK TO sp1;
来源：http://dxc.cashguo.top

[Q69] 查看执行计划
来源：http://tgz.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://emt.hnxiangtu.top

[Q70] 更新统计信息
来源：http://mhs.zhaomingkeji.xyz

ANALYZE TABLE users;
来源：http://wkm.guannengcc.top

[Q71] 查看建表语句
来源：http://jhi.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hpb.shanyushiyangkeji.top

[Q72] 查看索引
来源：http://tsp.haohaochexian.top

SHOW INDEX FROM users;
来源：http://dhq.meibo888.top

[Q73] 查看表状态
来源：http://kru.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vys.aizwys.cn

[Q74] 强制使用索引
来源：http://mwb.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fvn.chenlongwang.top

[Q75] 日期格式化
来源：http://shx.zhaomingkeji.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dkh.xylfe.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ksz.jinqigfzy.top

[Q76] 按天统计
来源：http://bjk.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oln.cashguo.top

[Q77] 时间加减
来源：http://zbc.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lli.jinghuilouyu.cn

[Q78] 当前时间
来源：http://voy.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hai.jlsjyb.cn

[Q79] 字符串拼接
来源：http://tvr.cashguo.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dip.yj202588.top

[Q80] 字符串截取
来源：http://trp.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uvs.hongshengwenyu.top

[Q81] 字符串替换
来源：http://xey.fktsv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vte.jinqigufen.top

[Q82] 字符长度与字节长度
来源：http://xwz.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wxm.hysaishi.cn

[Q83] 大小写转换
来源：http://ftc.xinyue.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ydg.hysaishi.cn

[Q84] 去除首尾空格
来源：http://iac.cdnleiting.top

SELECT TRIM(name) FROM users;
来源：http://tgz.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://clt.vehdjk.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mck.gogol.net.cn

[Q86] 读取 JSON 字段
来源：http://zft.tian-w.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oeu.yj20258888.top

[Q87] JSON 字段做条件
来源：http://drh.jinqigfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wcm.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://jtb.hcnkem.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ict.jlsjyb.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eab.aibaodan.cn

[Q89] 判断表是否存在
来源：http://sdl.xuanzx.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://itr.jinqigufen.top

[Q90] 生成序号列
来源：http://sec.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qbs.iojbl.cn

================================================================================
来源：http://ugp.yj20258.top

R. Bash 专题
来源：http://pdb.hongshengwenyu.top

================================================================================
来源：http://jfm.wangdashe.top

[R01] shebang 与严格模式
来源：http://ebm.tianlin.xyz

#!/usr/bin/env bash
来源：http://bhj.dianchejie.cn

set -euo pipefail
来源：http://kfk.daria6918.cn

[R02] 变量赋值与使用
来源：http://zzg.daxiang520.top

name="Tom"; echo "$name"
来源：http://jlm.zhaomingkeji.xyz

[R03] 只读变量
来源：http://ilb.yuxming.cn

readonly PI=3.14
来源：http://nbf.yj202588.top

[R04] 位置参数
来源：http://kdz.iojbl.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lyd.tarul.cn

[R05] 参数默认值
来源：http://jfb.tianlin.xyz

name="${1:-default}"
来源：http://bbg.epnwcf.com

[R06] 判断命令是否存在
来源：http://uan.jqgfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://esj.sweek.top

[R07] if 判断文件
来源：http://izb.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qxj.xingfuxueyuan.xyz

[R08] 数值比较
来源：http://cpi.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ahq.jqgufenzy.top

[R09] 字符串比较
来源：http://bue.xylfe.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gkc.hongshengwenyu.top

[R10] 正则匹配
来源：http://bxd.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ail.cashguo.top

[R11] case 多分支
来源：http://vsr.ywan-chungtsiang.top

case "$1" in
来源：http://fyq.uphjek.com

start) echo "启动" ;;
来源：http://hfr.yongpay.top

stop)  echo "停止" ;;
来源：http://tjv.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://gxk.smart0.xyz

esac
来源：http://iya.uphjek.com

[R12] for 遍历文件
来源：http://swt.svipenyu.cn

for f in *.txt; do echo "$f"; done
来源：http://jvm.kuanghao11.cn

[R13] for 计数循环
来源：http://znl.fanxiaobao.xyz

for i in {1..10}; do echo "$i"; done
来源：http://jtc.jqgfzy.top

[R14] C 风格 for
来源：http://edx.sweek.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qcl.ppjwa.cn

[R15] while 逐行读文件
来源：http://yic.ybcxt.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ulf.sysykeji.top

[R16] until 等待条件
来源：http://ekt.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gnk.tianlin.xyz

[R17] 数组定义与取值
来源：http://hkw.wangdashe.top

arr=(a b c); echo "${arr[0]}"
来源：http://akg.aizwys.cn

[R18] 遍历数组
来源：http://aca.c1oappe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wet.shuidangran.top

[R19] 数组长度
来源：http://kga.yfazqb.com

echo "${#arr[@]}"
来源：http://ivg.kuanghao11.cn

[R20] 关联数组（字典）
来源：http://jul.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dvf.andypj.xyz

[R21] 字符串长度
来源：http://iok.smart0.xyz

echo "${#s}"
来源：http://khk.snrcjt.cn

[R22] 截取子串
来源：http://jaw.chenlongwang.top

echo "${s:0:5}"
来源：http://kxu.hywenlv.cn

[R23] 字符串替换
来源：http://dcf.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yll.0kj1m.cn

[R24] 大小写转换
来源：http://lhb.shangyingyoupin.top

echo "${s^^}"; echo "${s,,}"
来源：http://ohg.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://yka.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zrl.zhixingplan.top

[R26] 命令替换
来源：http://ffo.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://fhd.iojbl.cn

[R27] 算术展开
来源：http://eue.yueranfly.top

echo $((1 + 2 * 3))
来源：http://avz.cqqwz.cn

[R28] 浮点运算
来源：http://gem.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://rbo.feifeiyinyue.top

[R29] 定义函数
来源：http://qsn.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://van.ivvv.top

[R30] 函数返回状态码
来源：http://hsg.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://ide.ydzc1.top

[R31] 局部变量
来源：http://vyu.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://spd.tianlin.xyz

[R32] 参数个数校验
来源：http://uba.meibo888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ktu.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://smv.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ycd.zhengqikj.top

[R34] 退出时清理
来源：http://yug.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://bre.jqgufenzy.top

[R35] 后台执行并等待
来源：http://bou.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bhk.nanxuanxn.top

[R36] 并发执行多个任务
来源：http://wav.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qwv.meibo888.top

[R37] 把输出赋给变量
来源：http://jzd.tarul.cn

files=$(ls -1)
来源：http://swc.zdqjudy.top

[R38] 管道串联
来源：http://pda.shanyushiyangtech.top

cat a.txt | grep -i error | wc -l
来源：http://vgn.yj20258.top

[R39] 重定向标准输出与错误
来源：http://huo.iojbl.cn

cmd > out.log 2>&1
来源：http://vky.sufxvd.cn

[R40] 追加写日志
来源：http://yhj.wangdashe.top

echo "log" >> out.log
来源：http://ahs.gaohongyu789.top

[R41] 丢弃输出
来源：http://cqm.tarul.cn

cmd >/dev/null 2>&1
来源：http://kva.aizwys.cn

[R42] 输入重定向
来源：http://ugf.cucudq.cn

wc -l < a.txt
来源：http://kik.yangfankeji.com

[R43] 按名字查找文件
来源：http://cjv.ctjpmb.com

find . -name "*.log" -type f
来源：http://vqa.cdnleiting.top

[R44] 按修改时间查找
来源：http://bae.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://lqb.gaohongyu789.top

[R45] 批量删除
来源：http://xxb.shuidangran.top

find . -name "*.tmp" -delete
来源：http://enr.yueranfly.top

[R46] 递归替换文件内容
来源：http://nkf.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://shv.ctjpmb.com

[R47] sed 单行替换
来源：http://tyh.smart0.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://fdj.ybcxt.top

[R48] awk 取指定列
来源：http://wss.hcnkem.com

awk '{print $1, $3}' a.txt
来源：http://rnm.cucudq.cn

[R49] awk 带条件
来源：http://xit.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lbr.ydzc1.top

[R50] awk 求和
来源：http://aul.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mfn.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://hcj.svipenyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://esm.fanxiaobao.xyz

[R52] 统计行数
来源：http://yam.jinghuilouyu.cn

wc -l a.txt
来源：http://uaq.ppjwa.cn

[R53] 查看文件头与实时尾
来源：http://unq.xingfuxueyuan.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mxm.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://amm.vqdsnc.cn

diff a.txt b.txt
来源：http://dkn.sysykeji.top

[R55] 压缩与解压
来源：http://oyl.ppjwa.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ykf.svipenyu.cn

[R56] 远程拷贝
来源：http://mts.quarkkingdee.top

scp file user@host:/path/
来源：http://ntl.bbcook.cn

[R57] 远程执行命令
来源：http://skk.snrcjt.cn

ssh user@host 'uptime'
来源：http://eiz.yuanzhike.top

[R58] 下载文件
来源：http://dzm.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vvo.zdbjq.cn

[R59] 发 POST JSON
来源：http://wki.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ior.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://yby.hywenlv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://doe.ctjpmb.com

[R61] 磁盘占用
来源：http://ayi.zhiwuduotai.top

df -h;  du -sh *
来源：http://ynr.ctjpmb.com

[R62] 找最占空间的文件
来源：http://sdz.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://ncb.daria6918.cn

[R63] 内存与进程
来源：http://gcu.bjfxy.top

free -h;  ps aux | grep nginx
来源：http://tzi.ehwqpu.com

[R64] 结束进程
来源：http://tnf.jianghu66.top

kill -9 $(pgrep -f app.py)
来源：http://kkp.ybcxt.top

[R65] 查看端口占用
来源：http://iae.52xcode.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xpe.meibo888.top

[R66] 定时任务
来源：http://chv.fktsv.cn

crontab -e;  crontab -l
来源：http://hqv.iojbl.cn

[R67] 生成随机十六进制串
来源：http://qxr.jlsjyb.cn

openssl rand -hex 16
来源：http://ekh.ctjpmb.com

[R68] 计算文件校验值
来源：http://oof.hammf.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lji.quarkkingdee.top

[R69] 生成随机密码
来源：http://qkx.c1oappe.top

head -c 16 /dev/urandom | base64
来源：http://bdc.gaohongyu789.top

[R70] 时间戳与互转
来源：http://sfm.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://nhy.fanxiaobao.xyz

[R71] 日期格式化
来源：http://eye.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mav.chenjidiqi.icu

[R72] 等待端口就绪
来源：http://wyt.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cam.0kj1m.cn

[R73] 分割大日志
来源：http://qbi.bbcook.cn

split -l 1000 big.log part_
来源：http://qqk.xuetiantiany.cn

[R74] 批量重命名
来源：http://zwe.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lwg.dianchejie.cn

[R75] 导出环境变量
来源：http://pfl.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://tqd.cucudq.cn

[R76] 使用临时文件
来源：http://gvr.birdmap.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://liv.fzhhl.top

[R77] 读取用户输入
来源：http://wdr.havefunace.top

read -rp "请输入: " ans
来源：http://vco.gaohongyu789.top

[R78] 交互式菜单
来源：http://ocy.316326.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://qxa.jqgufenzy.top

[R79] 解析命令行选项
来源：http://kfj.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://avf.hysaishi.cn

[R80] 查看脚本执行耗时
来源：http://szp.cucudq.cn

time ./run.sh
来源：http://yqw.daxiang520.top

================================================================================
来源：http://sjd.dashuyun.cn

S. C / C++ 专题
来源：http://xrg.cashguo.top

================================================================================
来源：http://frk.cashguo.top

[S01] C：Hello World
来源：http://sps.sxryk.cn

#include <stdio.h>
来源：http://inu.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jcc.shangyingyoupin.top

[S02] C：变量与格式化输出
来源：http://gte.zhixingplan.top

int a = 10; printf("%d\n", a);
来源：http://bqj.jinqigfzy.top

[S03] C：读入整数
来源：http://zsq.cashguo.top

int x; scanf("%d", &x);
来源：http://qoh.epnwcf.com

[S04] C：字符串复制
来源：http://fae.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://kaq.chenlongwang.top

[S05] C：字符串长度
来源：http://iff.sjlbkw.cn

strlen(s)
来源：http://duy.daria6918.cn

[S06] C：字符串比较
来源：http://dip.hnxiangtu.top

strcmp(a, b) == 0
来源：http://ggy.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://qlt.hfpthk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ccd.yj20258.top

[S08] C：动态内存分配与释放
来源：http://vty.jqgufenzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hkl.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://vxa.316326.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ohc.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://idw.sjlbkw.cn

int *p = &a;  *p = 5;
来源：http://mdy.yuxming.cn

[S11] C：逐行读文件
来源：http://zly.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "r");
来源：http://ddy.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kiz.havefunace.top

fclose(f);
来源：http://kdc.feifeiyinyue.top

[S12] C：写文件
来源：http://edz.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ixc.hesvh.cn

[S13] C：宏定义
来源：http://xsv.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qfw.shuidangran.top

[S14] C：枚举
来源：http://bnf.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://oks.ctjpmb.com

[S15] C：类型转换
来源：http://ofb.pengpengdd.cyou

(double) a / b
来源：http://cwb.hywenlv.cn

[S16] C：位操作置位
来源：http://qvs.tian-w.cn

x |= (1 << 3);
来源：http://ynn.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://zhl.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gld.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://zds.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://psh.yongpay.top

[S19] C：快速排序
来源：http://roe.vehdjk.com

qsort(a, n, sizeof(int), cmp);
来源：http://vqm.yvedp.cn

[S20] C：二分查找
来源：http://kbu.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jiy.aibaodan.cn

[S21] C：字符类别判断
来源：http://ncj.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://byl.hywenlv.cn

[S22] C：字符串转数字
来源：http://iea.sufxvd.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qvn.ivvv.top

[S23] C：随机数
来源：http://xrp.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ctp.hywenlv.cn

[S24] C：获取本地时间
来源：http://mde.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://npz.ivvv.top

[S25] C：内存拷贝
来源：http://ckw.yongpay.top

memcpy(dst, src, n);
来源：http://uvl.vqdsnc.cn

[S26] C：内存清零
来源：http://ksj.yangfankeji.com


<!-- 参考信息 -->