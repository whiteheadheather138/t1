代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qrw.yanxiufei.cn

[Q54] 清空表
来源：http://dbi.shangyingyoupin.top

TRUNCATE TABLE logs;
来源：http://frn.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://odc.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://axq.ydzc1.top

[Q56] 密集排名（并列不占位）
来源：http://jql.yvedp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lej.fzhhl.top

[Q57] 行号
来源：http://wic.wangdashe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://asc.hywenlv.cn

[Q58] 累计求和
来源：http://qvw.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jks.jinyuanbaomall.cn

[Q59] 分组内累计
来源：http://dox.cqqwz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fkr.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://nlm.yanxiufei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://neb.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cxt.c1oappe.top

[Q61] 移动平均
来源：http://yas.yanxiufei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bos.bjfxy.top

[Q62] 分组占比
来源：http://ygb.fanxiaobao.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kuv.bjfxy.top

[Q63] 开启事务
来源：http://jrf.yonumen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ron.shuidangran.top

[Q64] 提交事务
来源：http://uza.feifeiyinyue.top

COMMIT;
来源：http://fbb.nanxinkj.top

[Q65] 回滚事务
来源：http://ski.havefunace.top

ROLLBACK;
来源：http://gow.pengpengdd.cyou

[Q66] 行锁查询
来源：http://skz.tianlin.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://edt.zycfv.cn

[Q67] 设置隔离级别
来源：http://rka.sxryk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qlv.zycfv.cn

[Q68] 保存点
来源：http://gfn.sysykeji.top

SAVEPOINT sp1;
来源：http://hkb.aizwys.cn

ROLLBACK TO sp1;
来源：http://swd.yj20258888.top

[Q69] 查看执行计划
来源：http://kph.sufxvd.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wtl.yj20258888.top

[Q70] 更新统计信息
来源：http://sjc.pycfn.com

ANALYZE TABLE users;
来源：http://nxq.bjfxy.top

[Q71] 查看建表语句
来源：http://zos.cucudq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hbu.iojbl.cn

[Q72] 查看索引
来源：http://kqm.xingfuxueyuan.xyz

SHOW INDEX FROM users;
来源：http://jtg.9152youxi.cn

[Q73] 查看表状态
来源：http://mbo.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pud.sysykeji.top

[Q74] 强制使用索引
来源：http://hie.andypj.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ntw.snrcjt.cn

[Q75] 日期格式化
来源：http://bfy.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bde.yj20258888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tlf.jinqigfzy.top

[Q76] 按天统计
来源：http://rcz.nanxuanxn.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kqe.yueranfly.top

[Q77] 时间加减
来源：http://uem.shuidangran.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://psr.sweek.top

[Q78] 当前时间
来源：http://rhu.shzxlz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mqc.jinyuanbaomall.cn

[Q79] 字符串拼接
来源：http://uju.yj20258.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zpl.chenjidiqi.icu

[Q80] 字符串截取
来源：http://tis.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wbc.birdmap.top

[Q81] 字符串替换
来源：http://ecn.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wcc.cheryme.top

[Q82] 字符长度与字节长度
来源：http://kuf.sjlbkw.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ivf.quarkkingdee.top

[Q83] 大小写转换
来源：http://upt.zhongyouzk.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jvt.wangdashe.top

[Q84] 去除首尾空格
来源：http://izj.gotoacloud.top

SELECT TRIM(name) FROM users;
来源：http://fyd.guowangkeji.top

[Q85] 数值取整
来源：http://hrl.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lkb.hongshengwenyu.top

[Q86] 读取 JSON 字段
来源：http://wgq.yongpay.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ffw.bbcook.cn

[Q87] JSON 字段做条件
来源：http://vfd.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aqn.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://bxo.shangyingyoupin.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sea.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://crn.ydzc1.top

[Q89] 判断表是否存在
来源：http://krm.sysykeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mzk.yuxming.cn

[Q90] 生成序号列
来源：http://qzi.chenjidiqi.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ifw.kuanghao11.cn

================================================================================
来源：http://fxt.jqgfzy.top

R. Bash 专题
来源：http://dzi.feifeiyinyue.top

================================================================================
来源：http://kwj.jinghuilouyu.cn

[R01] shebang 与严格模式
来源：http://bnp.316326.xyz

#!/usr/bin/env bash
来源：http://vtd.cucudq.cn

set -euo pipefail
来源：http://dtp.nanxuanxn.top

[R02] 变量赋值与使用
来源：http://amf.hcnkem.com

name="Tom"; echo "$name"
来源：http://dad.zhiwuduotai.top

[R03] 只读变量
来源：http://vrq.uphjek.com

readonly PI=3.14
来源：http://civ.yfazqb.com

[R04] 位置参数
来源：http://mou.chenzaomai.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vwh.gzhubu.top

[R05] 参数默认值
来源：http://qhv.52xcode.cn

name="${1:-default}"
来源：http://vhe.smart0.xyz

[R06] 判断命令是否存在
来源：http://vpa.ehwqpu.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ffw.yongpay.top

[R07] if 判断文件
来源：http://frn.yuanzhike.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://igb.yuanzhike.top

[R08] 数值比较
来源：http://ccl.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://brh.tanke756.top

[R09] 字符串比较
来源：http://ajn.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://npt.ybcxt.top

[R10] 正则匹配
来源：http://qep.vqdsnc.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://krj.bbcook.cn

[R11] case 多分支
来源：http://gwo.haohaochexian.top

case "$1" in
来源：http://xpk.sysykeji.top

start) echo "启动" ;;
来源：http://xyi.mhx1999.top

stop)  echo "停止" ;;
来源：http://cqp.aizwys.cn

*)     echo "未知命令" ;;
来源：http://tjs.yanxiufei.cn

esac
来源：http://xew.jiagoushi.top

[R12] for 遍历文件
来源：http://crc.hfpthk.cn

for f in *.txt; do echo "$f"; done
来源：http://eyj.zhoulong.xyz

[R13] for 计数循环
来源：http://nml.sjlbkw.cn

for i in {1..10}; do echo "$i"; done
来源：http://qnc.ehwqpu.com

[R14] C 风格 for
来源：http://shn.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bog.xinyue.icu

[R15] while 逐行读文件
来源：http://bxh.mhx1999.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ahh.fzhhl.top

[R16] until 等待条件
来源：http://wpl.snrcjt.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kku.aibaodan.cn

[R17] 数组定义与取值
来源：http://vxu.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://gut.ppjwa.cn

[R18] 遍历数组
来源：http://zgo.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://caz.meibo888.top

[R19] 数组长度
来源：http://slr.cqqwz.cn

echo "${#arr[@]}"
来源：http://kqm.iojbl.cn

[R20] 关联数组（字典）
来源：http://rme.hfpthk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wtx.jqgfzy.top

[R21] 字符串长度
来源：http://dzn.c1oappe.top

echo "${#s}"
来源：http://kfc.dashuyun.cn

[R22] 截取子串
来源：http://xrh.aibaodan.cn

echo "${s:0:5}"
来源：http://lqh.jiagoushi.top

[R23] 字符串替换
来源：http://lkv.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pfm.jinqigfzy.top

[R24] 大小写转换
来源：http://pqy.redwolf501.top

echo "${s^^}"; echo "${s,,}"
来源：http://oif.zhijiandao.cn

[R25] 去后缀 / 去前缀
来源：http://lvy.jiagoushi.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vsc.zycfv.cn

[R26] 命令替换
来源：http://rvv.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://miz.ctjpmb.com

[R27] 算术展开
来源：http://efv.aibaodan.cn

echo $((1 + 2 * 3))
来源：http://kgv.jiagoushi.top

[R28] 浮点运算
来源：http://hea.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://waf.ppjwa.cn

[R29] 定义函数
来源：http://xiv.0kj1m.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mtt.fzhhl.top

[R30] 函数返回状态码
来源：http://gcz.yfazqb.com

f() { return 0; }; f || echo "失败了"
来源：http://gle.yangfankeji.com

[R31] 局部变量
来源：http://ekb.daxiang520.top

f() { local x=1; echo "$x"; }
来源：http://ikv.cashguo.top

[R32] 参数个数校验
来源：http://lri.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bnr.yonumen.top

[R33] 捕获错误并提示行号
来源：http://dxw.redwolf501.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ffg.yangfankeji.com

[R34] 退出时清理
来源：http://ref.gogol.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wzh.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://hqb.hongshengwenyu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mlw.epnwcf.com

[R36] 并发执行多个任务
来源：http://xfn.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jdr.aibaodan.cn

[R37] 把输出赋给变量
来源：http://rpo.yj20258.top

files=$(ls -1)
来源：http://pyy.gotoacloud.top

[R38] 管道串联
来源：http://jtb.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://elk.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://uwv.9152youxi.cn

cmd > out.log 2>&1
来源：http://fqr.wangshuangyany.cn

[R40] 追加写日志
来源：http://uee.yvedp.cn

echo "log" >> out.log
来源：http://epk.sjlbkw.cn

[R41] 丢弃输出
来源：http://fgf.daxiang520.top

cmd >/dev/null 2>&1
来源：http://oih.fengsongda.top

[R42] 输入重定向
来源：http://whd.chenzaomai.com

wc -l < a.txt
来源：http://wqf.pycfn.com

[R43] 按名字查找文件
来源：http://jir.xziqi.cn

find . -name "*.log" -type f
来源：http://mkt.kuanghao11.cn

[R44] 按修改时间查找
来源：http://ztr.daxiang520.top

find . -mtime -7 -type f
来源：http://yfs.redwolf501.top

[R45] 批量删除
来源：http://mpk.316326.xyz

find . -name "*.tmp" -delete
来源：http://eob.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://tri.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ozu.0kj1m.cn

[R47] sed 单行替换
来源：http://rky.shanyushiyangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://prr.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://fbm.nanxuanxn.top

awk '{print $1, $3}' a.txt
来源：http://dox.hammf.cn

[R49] awk 带条件
来源：http://gnx.jqgfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ukz.ywan-chungtsiang.top

[R50] awk 求和
来源：http://iud.jyoumei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://foz.sufxvd.cn

[R51] 排序去重取前几
来源：http://qxt.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mnm.bjfxy.top

[R52] 统计行数
来源：http://qzj.jinghuilouyu.cn

wc -l a.txt
来源：http://zht.yj202588.top

[R53] 查看文件头与实时尾
来源：http://vgn.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dex.cashguo.top

[R54] 比较两个文件
来源：http://bfr.ydjk.org.cn

diff a.txt b.txt
来源：http://zap.hcnkem.com

[R55] 压缩与解压
来源：http://koq.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iop.ehwqpu.com

[R56] 远程拷贝
来源：http://fko.zhoulong.xyz

scp file user@host:/path/
来源：http://mpq.ppjwa.cn

[R57] 远程执行命令
来源：http://yys.cheryme.top

ssh user@host 'uptime'
来源：http://qkt.nanxinkj.top

[R58] 下载文件
来源：http://sof.nanxuanxn.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ruy.gzhubu.top

[R59] 发 POST JSON
来源：http://ren.ehwqpu.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pls.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://isa.fanxiaobao.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://czi.zhengqikj.top

[R61] 磁盘占用
来源：http://iyi.hnxiangtu.top

df -h;  du -sh *
来源：http://xpf.tarul.cn

[R62] 找最占空间的文件
来源：http://rtu.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://sfp.daria6918.cn

[R63] 内存与进程
来源：http://hgv.uphjek.com

free -h;  ps aux | grep nginx
来源：http://ito.yueranfly.top

[R64] 结束进程
来源：http://alx.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://asx.yueranfly.top

[R65] 查看端口占用
来源：http://omg.gaohongyu789.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wst.svipenyu.cn

[R66] 定时任务
来源：http://wag.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://upd.c1oappe.top

[R67] 生成随机十六进制串
来源：http://nrk.tianlin.xyz

openssl rand -hex 16
来源：http://eyi.ydzc1.top

[R68] 计算文件校验值
来源：http://hqd.gaohongyu789.top

sha256sum a.txt;  md5sum a.txt
来源：http://beg.nanxinkj.top

[R69] 生成随机密码
来源：http://yob.ehwqpu.com

head -c 16 /dev/urandom | base64
来源：http://bry.haohaochexian.top

[R70] 时间戳与互转
来源：http://sbn.yfazqb.com

date +%s;  date -d @1700000000
来源：http://ajv.yfazqb.com

[R71] 日期格式化
来源：http://dko.pycfn.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://uwa.316326.xyz

[R72] 等待端口就绪
来源：http://uvv.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vtx.jlsjyb.cn

[R73] 分割大日志
来源：http://bcg.hysaishi.cn

split -l 1000 big.log part_
来源：http://uxo.sysykeji.top

[R74] 批量重命名
来源：http://mki.epnwcf.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bpa.iojbl.cn

[R75] 导出环境变量
来源：http://wum.zhixingplan.top

export PATH="$HOME/bin:$PATH"
来源：http://mui.yangfankeji.com

[R76] 使用临时文件
来源：http://ovb.ehwqpu.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wsw.ybcxt.top

[R77] 读取用户输入
来源：http://yqj.fzhhl.top

read -rp "请输入: " ans
来源：http://jdr.vehdjk.com

[R78] 交互式菜单
来源：http://exy.xylfe.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cbj.hnxiangtu.top

[R79] 解析命令行选项
来源：http://ncd.yj202588.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://skk.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://vst.tian-w.cn

time ./run.sh
来源：http://nhc.ydjk.org.cn

================================================================================
来源：http://giv.iojbl.cn

S. C / C++ 专题
来源：http://sjn.cashguo.top

================================================================================
来源：http://apb.tarul.cn

[S01] C：Hello World
来源：http://mvu.haohaochexian.top

#include <stdio.h>
来源：http://uft.yuxming.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wxs.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://kbj.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://tsb.fanxiaobao.xyz

[S03] C：读入整数
来源：http://ewx.cqqwz.cn

int x; scanf("%d", &x);
来源：http://ung.hysaishi.cn

[S04] C：字符串复制
来源：http://fij.nwbrower.top

char dst[32]; strcpy(dst, "hi");
来源：http://bbo.cashguo.top

[S05] C：字符串长度
来源：http://odj.nanxinkj.top

strlen(s)
来源：http://udi.epnwcf.com

[S06] C：字符串比较
来源：http://yrr.daria6918.cn

strcmp(a, b) == 0
来源：http://jfg.nwbrower.top

[S07] C：数组遍历求和
来源：http://njn.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uwz.sxryk.cn

[S08] C：动态内存分配与释放
来源：http://xwv.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cfi.jinyuanbaomall.cn

[S09] C：结构体定义与初始化
来源：http://uss.uphjek.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kwd.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://fxc.daria6918.cn

int *p = &a;  *p = 5;
来源：http://rmo.kuanghao11.cn

[S11] C：逐行读文件
来源：http://lee.pengpengdd.cyou

FILE *f = fopen("a.txt", "r");
来源：http://nhd.jianghu66.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ipn.tianlin.xyz

fclose(f);
来源：http://nka.zhiwuduotai.top

[S12] C：写文件
来源：http://hpf.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jsx.gaohongyu789.top

[S13] C：宏定义
来源：http://dls.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://reo.cashguo.top

[S14] C：枚举
来源：http://nsr.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://xrd.tian-w.cn

[S15] C：类型转换
来源：http://fzi.gaohongyu789.top

(double) a / b
来源：http://rwq.gotoacloud.top

[S16] C：位操作置位
来源：http://iyp.shanyushiyangtech.top

x |= (1 << 3);
来源：http://wac.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://avi.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sik.nwbrower.top

[S18] C：命令行参数
来源：http://qxu.0kj1m.cn

int main(int argc, char **argv)
来源：http://gkl.zhiwuduotai.top

[S19] C：快速排序
来源：http://smk.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://fxm.jqgufenzy.top

[S20] C：二分查找
来源：http://tlu.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hvm.yangfankeji.com

[S21] C：字符类别判断
来源：http://sqv.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vkd.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://rxw.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://xch.gzhubu.top

[S23] C：随机数
来源：http://kny.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fle.zhixingplan.top

[S24] C：获取本地时间
来源：http://twp.birdmap.top


<!-- 参考信息 -->