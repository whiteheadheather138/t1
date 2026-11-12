代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ksn.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://jff.fehbvm.com

DELETE FROM users WHERE id = 10;
来源：http://bzb.jqgufenzy.top

[Q53] 按条件删除
来源：http://pqx.kuanghao11.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cun.sjlbkw.cn

[Q54] 清空表
来源：http://yno.jyoumei.cn

TRUNCATE TABLE logs;
来源：http://oxl.sysykeji.top

[Q55] 排名（并列占位）
来源：http://lkg.aizwys.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uka.jqgufenzy.top

[Q56] 密集排名（并列不占位）
来源：http://slr.hnxiangtu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vnu.zhiwuduotai.top

[Q57] 行号
来源：http://sir.ppjwa.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gng.bjfxy.top

[Q58] 累计求和
来源：http://hqi.tianlin.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nxm.pycfn.com

[Q59] 分组内累计
来源：http://phr.yongpay.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nmz.hesvh.cn

[Q60] 取上一行 / 下一行
来源：http://rhk.hongshengwenyu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://chx.redwolf501.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pit.fengsongda.top

[Q61] 移动平均
来源：http://qzb.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vly.tanke756.top

[Q62] 分组占比
来源：http://eny.zhijiandao.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://utv.pycfn.com

[Q63] 开启事务
来源：http://rvd.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://mdj.haohaochexian.top

[Q64] 提交事务
来源：http://cys.ivvv.top

COMMIT;
来源：http://kyq.xuetiantiany.cn

[Q65] 回滚事务
来源：http://elq.316326.xyz

ROLLBACK;
来源：http://qkw.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://ojx.cashguo.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rhz.nanxuanxn.top

[Q67] 设置隔离级别
来源：http://epu.shzxlz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://luy.yueranfly.top

[Q68] 保存点
来源：http://vyk.xuetiantiany.cn

SAVEPOINT sp1;
来源：http://dhs.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://agl.fzhhl.top

[Q69] 查看执行计划
来源：http://pth.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://edi.sxryk.cn

[Q70] 更新统计信息
来源：http://moy.zhengqikj.top

ANALYZE TABLE users;
来源：http://ohy.aizwys.cn

[Q71] 查看建表语句
来源：http://sri.c1oappe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wrp.ctjpmb.com

[Q72] 查看索引
来源：http://ifi.tarul.cn

SHOW INDEX FROM users;
来源：http://dyj.yanxiufei.cn

[Q73] 查看表状态
来源：http://gzp.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xpi.fengsongda.top

[Q74] 强制使用索引
来源：http://udu.hfpthk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ulj.zycfv.cn

[Q75] 日期格式化
来源：http://yrw.dianchejie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cux.snrcjt.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://efc.havefunace.top

[Q76] 按天统计
来源：http://jyu.tian-w.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://etp.jinyuanbaomall.cn

[Q77] 时间加减
来源：http://tlz.uphjek.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sxw.yanxiufei.cn

[Q78] 当前时间
来源：http://vwh.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tln.hnxiangtu.top

[Q79] 字符串拼接
来源：http://wme.bbcook.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://avs.zhengqikj.top

[Q80] 字符串截取
来源：http://obd.hnxiangtu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://phu.cdnleiting.top

[Q81] 字符串替换
来源：http://ziy.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://plz.c1oappe.top

[Q82] 字符长度与字节长度
来源：http://opt.mhx1999.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qbp.bbcook.cn

[Q83] 大小写转换
来源：http://yjo.shanyushiyangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gwb.jinqigfzy.top

[Q84] 去除首尾空格
来源：http://cda.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://tbk.sxryk.cn

[Q85] 数值取整
来源：http://jri.yuxming.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mmp.cashguo.top

[Q86] 读取 JSON 字段
来源：http://eti.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xjj.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://pmm.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cud.0kj1m.cn

[Q88] 行转列（条件聚合）
来源：http://rnv.xingfuxueyuan.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://srx.zhongyouzk.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oma.hywenlv.cn

[Q89] 判断表是否存在
来源：http://gjt.zhijiandao.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ucs.shanyushiyangkeji.top

[Q90] 生成序号列
来源：http://jqo.dianchejie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nfy.zhaomingkeji.xyz

================================================================================
来源：http://pcv.xuetiantiany.cn

R. Bash 专题
来源：http://bex.dashuyun.cn

================================================================================
来源：http://zwy.sysykeji.top

[R01] shebang 与严格模式
来源：http://kfw.0kj1m.cn

#!/usr/bin/env bash
来源：http://hww.ywan-chungtsiang.top

set -euo pipefail
来源：http://lju.jinqigufen.top

[R02] 变量赋值与使用
来源：http://avp.jinghuilouyu.cn

name="Tom"; echo "$name"
来源：http://cbo.vehdjk.com

[R03] 只读变量
来源：http://hyt.yonumen.top

readonly PI=3.14
来源：http://ztf.epnwcf.com

[R04] 位置参数
来源：http://usp.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dfe.fktsv.cn

[R05] 参数默认值
来源：http://wxu.ehwqpu.com

name="${1:-default}"
来源：http://eew.yfazqb.com

[R06] 判断命令是否存在
来源：http://sxe.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nex.xuetiantiany.cn

[R07] if 判断文件
来源：http://jkd.zdqjudy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gqx.gogol.net.cn

[R08] 数值比较
来源：http://vnh.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://ikr.hcnkem.com

[R09] 字符串比较
来源：http://zvu.epnwcf.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hcc.zhengqikj.top

[R10] 正则匹配
来源：http://san.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rdi.hywenlv.cn

[R11] case 多分支
来源：http://aot.pengpengdd.cyou

case "$1" in
来源：http://brj.tian-w.cn

start) echo "启动" ;;
来源：http://hqg.9152youxi.cn

stop)  echo "停止" ;;
来源：http://rpd.nanxuanxn.top

*)     echo "未知命令" ;;
来源：http://kir.nanxuanxn.top

esac
来源：http://gva.shanyushiyangkeji.top

[R12] for 遍历文件
来源：http://kci.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://nbi.pycfn.com

[R13] for 计数循环
来源：http://ede.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://nco.hongshengwenyu.top

[R14] C 风格 for
来源：http://lmk.cdnleiting.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xjb.snrcjt.cn

[R15] while 逐行读文件
来源：http://orh.pengpengdd.cyou

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mlf.cqqwz.cn

[R16] until 等待条件
来源：http://vkv.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iky.sysykeji.top

[R17] 数组定义与取值
来源：http://ond.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://pzq.cheryme.top

[R18] 遍历数组
来源：http://jco.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ccw.ppjwa.cn

[R19] 数组长度
来源：http://cvp.tanke756.top

echo "${#arr[@]}"
来源：http://yxz.bbcook.cn

[R20] 关联数组（字典）
来源：http://ewa.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://spd.cashguo.top

[R21] 字符串长度
来源：http://xcx.jqgfzy.top

echo "${#s}"
来源：http://fun.snrcjt.cn

[R22] 截取子串
来源：http://iiy.vehdjk.com

echo "${s:0:5}"
来源：http://aju.tarul.cn

[R23] 字符串替换
来源：http://meb.dashuyun.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tti.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://crp.xylfe.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ran.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://oba.shanyushiyangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hlo.pycfn.com

[R26] 命令替换
来源：http://twf.sysykeji.top

now=$(date +%F); echo "$now"
来源：http://anr.dianchejie.cn

[R27] 算术展开
来源：http://hag.cucudq.cn

echo $((1 + 2 * 3))
来源：http://otx.52xcode.cn

[R28] 浮点运算
来源：http://vex.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://ogw.gotoacloud.top

[R29] 定义函数
来源：http://mun.hfpthk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zhx.haohaochexian.top

[R30] 函数返回状态码
来源：http://rso.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://aez.nanxuanxn.top

[R31] 局部变量
来源：http://ivz.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://dnh.jlsjyb.cn

[R32] 参数个数校验
来源：http://zad.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dcl.chenjidiqi.icu

[R33] 捕获错误并提示行号
来源：http://opc.pengpengdd.cyou

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xsz.jinqigfzy.top

[R34] 退出时清理
来源：http://vhw.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lpr.gogol.net.cn

[R35] 后台执行并等待
来源：http://jtc.jinyuanbaomall.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oiq.gaohongyu789.top

[R36] 并发执行多个任务
来源：http://grg.ydjk.org.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vpn.jinqigfzy.top

[R37] 把输出赋给变量
来源：http://wfo.zhixingplan.top

files=$(ls -1)
来源：http://ltp.chenlongwang.top

[R38] 管道串联
来源：http://spp.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://cjv.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://mbr.chenzaomai.com

cmd > out.log 2>&1
来源：http://ajh.9152youxi.cn

[R40] 追加写日志
来源：http://pkb.yanxiufei.cn

echo "log" >> out.log
来源：http://svc.9152youxi.cn

[R41] 丢弃输出
来源：http://urh.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://aud.shangyingyoupin.top

[R42] 输入重定向
来源：http://zfp.andypj.xyz

wc -l < a.txt
来源：http://fzu.bbcook.cn

[R43] 按名字查找文件
来源：http://avb.dianchejie.cn

find . -name "*.log" -type f
来源：http://pls.pycfn.com

[R44] 按修改时间查找
来源：http://ryh.dashuyun.cn

find . -mtime -7 -type f
来源：http://aku.aizwys.cn

[R45] 批量删除
来源：http://uwy.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://edj.xziqi.cn

[R46] 递归替换文件内容
来源：http://vmi.zdqjudy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://epp.ppjwa.cn

[R47] sed 单行替换
来源：http://fbp.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vto.tarul.cn

[R48] awk 取指定列
来源：http://ife.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://czb.nanxinkj.top

[R49] awk 带条件
来源：http://rkv.feifeiyinyue.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jtu.yueranfly.top

[R50] awk 求和
来源：http://pqa.jlsjyb.cn

awk '{s += $2} END {print s}' a.txt
来源：http://umi.0kj1m.cn

[R51] 排序去重取前几
来源：http://rhf.yuanzhike.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gjf.haohaochexian.top

[R52] 统计行数
来源：http://qun.yfazqb.com

wc -l a.txt
来源：http://ktd.jlsjyb.cn

[R53] 查看文件头与实时尾
来源：http://qti.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bft.yuxming.cn

[R54] 比较两个文件
来源：http://uwp.birdmap.top

diff a.txt b.txt
来源：http://dlt.hammf.cn

[R55] 压缩与解压
来源：http://hgx.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ktp.zhiwuduotai.top

[R56] 远程拷贝
来源：http://eur.cheryme.top

scp file user@host:/path/
来源：http://lal.snrcjt.cn

[R57] 远程执行命令
来源：http://wab.jinqigfzy.top

ssh user@host 'uptime'
来源：http://tyb.yj20258.top

[R58] 下载文件
来源：http://tzl.andypj.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://omi.shuidangran.top

[R59] 发 POST JSON
来源：http://qli.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dba.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://eif.zhaomingkeji.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kzw.jqgfzy.top

[R61] 磁盘占用
来源：http://owh.jiagoushi.top

df -h;  du -sh *
来源：http://iuk.tian-w.cn

[R62] 找最占空间的文件
来源：http://vkh.9152youxi.cn

du -ah . | sort -rh | head -10
来源：http://kss.yj20258888.top

[R63] 内存与进程
来源：http://dyj.zhoulong.xyz

free -h;  ps aux | grep nginx
来源：http://mep.guannengcc.top

[R64] 结束进程
来源：http://tnf.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://rfk.cucudq.cn

[R65] 查看端口占用
来源：http://yzl.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://skm.jqgufenzy.top

[R66] 定时任务
来源：http://omg.zycfv.cn

crontab -e;  crontab -l
来源：http://djd.52xcode.cn

[R67] 生成随机十六进制串
来源：http://ena.kuanghao11.cn

openssl rand -hex 16
来源：http://wyf.aizwys.cn

[R68] 计算文件校验值
来源：http://fyd.cucudq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ejn.0kj1m.cn

[R69] 生成随机密码
来源：http://fiu.tarul.cn

head -c 16 /dev/urandom | base64
来源：http://qax.tianlin.xyz

[R70] 时间戳与互转
来源：http://bvw.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://qvd.gogol.net.cn

[R71] 日期格式化
来源：http://eox.hammf.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xpe.jinqigufen.top

[R72] 等待端口就绪
来源：http://cze.jinqigfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mrw.mhx1999.top

[R73] 分割大日志
来源：http://cgz.wangshuangyany.cn

split -l 1000 big.log part_
来源：http://gwt.jyoumei.cn

[R74] 批量重命名
来源：http://dof.9152youxi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hxn.tianlin.xyz

[R75] 导出环境变量
来源：http://jfh.jinqigufen.top

export PATH="$HOME/bin:$PATH"
来源：http://elg.fehbvm.com

[R76] 使用临时文件
来源：http://zlw.dashuyun.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mno.chenlongwang.top

[R77] 读取用户输入
来源：http://xyw.sjlbkw.cn

read -rp "请输入: " ans
来源：http://fwu.zhoulong.xyz

[R78] 交互式菜单
来源：http://ubx.ehwqpu.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ohb.bjfxy.top

[R79] 解析命令行选项
来源：http://ebd.hysaishi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mkh.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://rkb.fengsongda.top

time ./run.sh
来源：http://dgk.ydjk.org.cn

================================================================================
来源：http://uyb.hysaishi.cn

S. C / C++ 专题
来源：http://npm.tarul.cn

================================================================================
来源：http://hpl.nanxuanxn.top

[S01] C：Hello World
来源：http://hdj.ywan-chungtsiang.top

#include <stdio.h>
来源：http://mlw.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://oyk.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://njs.jinqigufen.top

int a = 10; printf("%d\n", a);
来源：http://vmw.sjlbkw.cn

[S03] C：读入整数
来源：http://fmn.sufxvd.cn

int x; scanf("%d", &x);
来源：http://pnl.redwolf501.top

[S04] C：字符串复制
来源：http://vgo.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://icm.9152youxi.cn

[S05] C：字符串长度
来源：http://vhf.guowangkeji.top

strlen(s)
来源：http://wlf.hnqzz.top

[S06] C：字符串比较
来源：http://hxl.havefunace.top

strcmp(a, b) == 0
来源：http://bdl.c1oappe.top

[S07] C：数组遍历求和
来源：http://ynz.dianchejie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tib.hnqzz.top

[S08] C：动态内存分配与释放
来源：http://ovo.hesvh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uhm.zdbjq.cn

[S09] C：结构体定义与初始化
来源：http://rve.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bnv.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://lap.yj202588.top

int *p = &a;  *p = 5;
来源：http://nkm.gogol.net.cn

[S11] C：逐行读文件
来源：http://izh.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://exl.yanxiufei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vbt.svipenyu.cn

fclose(f);
来源：http://tll.fanxiaobao.xyz

[S12] C：写文件
来源：http://ryq.cqqwz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vxv.tarul.cn

[S13] C：宏定义
来源：http://otr.yj20258.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yzm.fanxiaobao.xyz

[S14] C：枚举
来源：http://glt.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://mga.jqgfzy.top

[S15] C：类型转换
来源：http://yqe.ivvv.top

(double) a / b
来源：http://xxa.hongshengwenyu.top

[S16] C：位操作置位
来源：http://obd.yuanzhike.top

x |= (1 << 3);
来源：http://eet.hnqzz.top

[S17] C：安全拼接字符串
来源：http://yxf.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aud.jinqigufen.top

[S18] C：命令行参数
来源：http://uth.yj20258.top

int main(int argc, char **argv)
来源：http://ifz.zhongyouzk.top

[S19] C：快速排序
来源：http://dtc.cucudq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mgd.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://upa.jqgfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mzz.gogol.net.cn

[S21] C：字符类别判断
来源：http://prv.cheryme.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ztg.c1oappe.top

[S22] C：字符串转数字
来源：http://swa.ywan-chungtsiang.top


<!-- 参考信息 -->