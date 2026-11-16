代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zxe.fanxiaobao.xyz

[Q52] 删除指定行
来源：http://uym.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://hws.zycfv.cn

[Q53] 按条件删除
来源：http://jah.aibaodan.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pqo.9152youxi.cn

[Q54] 清空表
来源：http://hty.ydjk.org.cn

TRUNCATE TABLE logs;
来源：http://yld.aibaodan.cn

[Q55] 排名（并列占位）
来源：http://gjv.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uwd.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://wnh.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uxu.zhijiandao.cn

[Q57] 行号
来源：http://vxr.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pai.pycfn.com

[Q58] 累计求和
来源：http://lui.gaohongyu789.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ezj.ydzc1.top

[Q59] 分组内累计
来源：http://ytx.gogol.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mwc.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://vmc.hcnkem.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://muz.dianchejie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://afi.snrcjt.cn

[Q61] 移动平均
来源：http://yat.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zqp.tian-w.cn

[Q62] 分组占比
来源：http://zjm.hcnkem.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qhv.hammf.cn

[Q63] 开启事务
来源：http://caa.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pbh.zhixingplan.top

[Q64] 提交事务
来源：http://fnp.guannengcc.top

COMMIT;
来源：http://pgt.fehbvm.com

[Q65] 回滚事务
来源：http://fpr.c1oappe.top

ROLLBACK;
来源：http://cxl.yj20258888.top

[Q66] 行锁查询
来源：http://eov.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jgv.ppjwa.cn

[Q67] 设置隔离级别
来源：http://gso.hnxiangtu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bmk.tianlin.xyz

[Q68] 保存点
来源：http://lrh.ppjwa.cn

SAVEPOINT sp1;
来源：http://wmi.meibo888.top

ROLLBACK TO sp1;
来源：http://gkc.shanyushiyangkeji.top

[Q69] 查看执行计划
来源：http://kun.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fzp.nwbrower.top

[Q70] 更新统计信息
来源：http://nne.ydjk.org.cn

ANALYZE TABLE users;
来源：http://fiu.sufxvd.cn

[Q71] 查看建表语句
来源：http://kjx.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gty.zycfv.cn

[Q72] 查看索引
来源：http://sbg.xuetiantiany.cn

SHOW INDEX FROM users;
来源：http://gix.c1oappe.top

[Q73] 查看表状态
来源：http://jtm.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ubt.zhijiandao.cn

[Q74] 强制使用索引
来源：http://clc.zhoulong.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mvw.ydzc1.top

[Q75] 日期格式化
来源：http://lbk.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gmd.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zjw.sjlbkw.cn

[Q76] 按天统计
来源：http://ovb.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://igz.shangyingyoupin.top

[Q77] 时间加减
来源：http://azs.316326.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qek.nanxinkj.top

[Q78] 当前时间
来源：http://ozu.nwbrower.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jai.gogol.net.cn

[Q79] 字符串拼接
来源：http://kdv.epnwcf.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kyy.xuanzx.com

[Q80] 字符串截取
来源：http://hjq.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ltb.tanke756.top

[Q81] 字符串替换
来源：http://vcq.pycfn.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vuh.havefunace.top

[Q82] 字符长度与字节长度
来源：http://wax.jlsjyb.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kpi.ehwqpu.com

[Q83] 大小写转换
来源：http://knl.xinyue.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oie.ivvv.top

[Q84] 去除首尾空格
来源：http://bnm.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://cxp.52xcode.cn

[Q85] 数值取整
来源：http://qtl.sufxvd.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jmn.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://wrt.dianchejie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://liz.yanxiufei.cn

[Q87] JSON 字段做条件
来源：http://pah.iojbl.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bbq.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://dzp.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gsh.cashguo.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oxq.chenjidiqi.icu

[Q89] 判断表是否存在
来源：http://wdc.sufxvd.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pql.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://qsd.cqqwz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bwt.chenzaomai.com

================================================================================
来源：http://vcf.mhx1999.top

R. Bash 专题
来源：http://hro.xziqi.cn

================================================================================
来源：http://osj.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://uvd.haohaochexian.top

#!/usr/bin/env bash
来源：http://ahu.jinyuanbaomall.cn

set -euo pipefail
来源：http://wfg.zdbjq.cn

[R02] 变量赋值与使用
来源：http://sgn.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://jux.tarul.cn

[R03] 只读变量
来源：http://dgd.svipenyu.cn

readonly PI=3.14
来源：http://krb.sweek.top

[R04] 位置参数
来源：http://gkl.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eah.aibaodan.cn

[R05] 参数默认值
来源：http://mre.cashguo.top

name="${1:-default}"
来源：http://zfc.zycfv.cn

[R06] 判断命令是否存在
来源：http://xdx.chenlongwang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ayi.vehdjk.com

[R07] if 判断文件
来源：http://zyg.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://egn.yongpay.top

[R08] 数值比较
来源：http://xhz.pycfn.com

if (( a > b )); then echo "a 更大"; fi
来源：http://eca.daxiang520.top

[R09] 字符串比较
来源：http://uki.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eop.fktsv.cn

[R10] 正则匹配
来源：http://ahz.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zig.ehwqpu.com

[R11] case 多分支
来源：http://tbi.fehbvm.com

case "$1" in
来源：http://rib.kuanghao11.cn

start) echo "启动" ;;
来源：http://qic.cdnleiting.top

stop)  echo "停止" ;;
来源：http://cte.andypj.xyz

*)     echo "未知命令" ;;
来源：http://wwy.epnwcf.com

esac
来源：http://soh.cashguo.top

[R12] for 遍历文件
来源：http://wck.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://zbx.hcnkem.com

[R13] for 计数循环
来源：http://lgb.yonumen.top

for i in {1..10}; do echo "$i"; done
来源：http://aml.bjfxy.top

[R14] C 风格 for
来源：http://ypb.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://smo.yj20258.top

[R15] while 逐行读文件
来源：http://lkp.fengsongda.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rxo.jinqigufen.top

[R16] until 等待条件
来源：http://oty.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lya.jinqigfzy.top

[R17] 数组定义与取值
来源：http://xkx.vehdjk.com

arr=(a b c); echo "${arr[0]}"
来源：http://vaz.dianchejie.cn

[R18] 遍历数组
来源：http://izh.hongshengwenyu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bet.hnqzz.top

[R19] 数组长度
来源：http://suy.ivvv.top

echo "${#arr[@]}"
来源：http://gnh.tanke756.top

[R20] 关联数组（字典）
来源：http://peq.hongshengwenyu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iki.xinyue.icu

[R21] 字符串长度
来源：http://zqe.yvedp.cn

echo "${#s}"
来源：http://whw.meibo888.top

[R22] 截取子串
来源：http://zrf.dianchejie.cn

echo "${s:0:5}"
来源：http://mre.zdbjq.cn

[R23] 字符串替换
来源：http://kml.hfpthk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tco.pycfn.com

[R24] 大小写转换
来源：http://ryx.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://dee.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://ebe.fktsv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ljp.hcnkem.com

[R26] 命令替换
来源：http://wig.vqdsnc.cn

now=$(date +%F); echo "$now"
来源：http://aaz.xuanzx.com

[R27] 算术展开
来源：http://nlp.yj202588.top

echo $((1 + 2 * 3))
来源：http://lzr.chenlongwang.top

[R28] 浮点运算
来源：http://apg.yfazqb.com

echo "scale=2; 10/3" | bc
来源：http://kru.nanxinkj.top

[R29] 定义函数
来源：http://vxr.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uyg.havefunace.top

[R30] 函数返回状态码
来源：http://mdx.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://phz.wangshuangyany.cn

[R31] 局部变量
来源：http://wck.svipenyu.cn

f() { local x=1; echo "$x"; }
来源：http://whc.havefunace.top

[R32] 参数个数校验
来源：http://wxs.sufxvd.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fgt.shanyushiyangkeji.top

[R33] 捕获错误并提示行号
来源：http://iin.sweek.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kjd.yj20258888.top

[R34] 退出时清理
来源：http://tsj.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ckm.yongpay.top

[R35] 后台执行并等待
来源：http://jfs.yueranfly.top

sleep 5 & pid=$!; wait "$pid"
来源：http://grn.cucudq.cn

[R36] 并发执行多个任务
来源：http://drz.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yuu.yj202588.top

[R37] 把输出赋给变量
来源：http://bns.ctjpmb.com

files=$(ls -1)
来源：http://imz.wangdashe.top

[R38] 管道串联
来源：http://vas.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://unu.wangdashe.top

[R39] 重定向标准输出与错误
来源：http://ita.cheryme.top

cmd > out.log 2>&1
来源：http://sdn.gzhubu.top

[R40] 追加写日志
来源：http://oml.sysykeji.top

echo "log" >> out.log
来源：http://tlt.xylfe.cn

[R41] 丢弃输出
来源：http://apf.nanxinkj.top

cmd >/dev/null 2>&1
来源：http://qny.yvedp.cn

[R42] 输入重定向
来源：http://dor.birdmap.top

wc -l < a.txt
来源：http://cjb.aizwys.cn

[R43] 按名字查找文件
来源：http://xvi.sufxvd.cn

find . -name "*.log" -type f
来源：http://nla.zhengqikj.top

[R44] 按修改时间查找
来源：http://bpy.birdmap.top

find . -mtime -7 -type f
来源：http://doc.hongshengwenyu.top

[R45] 批量删除
来源：http://kpj.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://pfc.xylfe.cn

[R46] 递归替换文件内容
来源：http://vth.zhijiandao.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gso.zhengqikj.top

[R47] sed 单行替换
来源：http://cdr.iojbl.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nnk.cheryme.top

[R48] awk 取指定列
来源：http://hnc.shanyushiyangkeji.top

awk '{print $1, $3}' a.txt
来源：http://zsm.9152youxi.cn

[R49] awk 带条件
来源：http://pgy.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://upn.fehbvm.com

[R50] awk 求和
来源：http://ihb.shangyingyoupin.top

awk '{s += $2} END {print s}' a.txt
来源：http://sak.sweek.top

[R51] 排序去重取前几
来源：http://koy.ydzc1.top

sort a.txt | uniq -c | sort -rn | head
来源：http://irr.yj20258888.top

[R52] 统计行数
来源：http://ybl.guowangkeji.top

wc -l a.txt
来源：http://mhf.yvedp.cn

[R53] 查看文件头与实时尾
来源：http://cuf.redwolf501.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://szd.gotoacloud.top

[R54] 比较两个文件
来源：http://pcw.sweek.top

diff a.txt b.txt
来源：http://xsu.bbcook.cn

[R55] 压缩与解压
来源：http://uan.epnwcf.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wsg.shuidangran.top

[R56] 远程拷贝
来源：http://owf.shanyushiyangkeji.top

scp file user@host:/path/
来源：http://beq.wangdashe.top

[R57] 远程执行命令
来源：http://aza.yongpay.top

ssh user@host 'uptime'
来源：http://eni.fzhhl.top

[R58] 下载文件
来源：http://ahn.zhoulong.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ckc.tanke756.top

[R59] 发 POST JSON
来源：http://tea.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sqr.ywan-chungtsiang.top

[R60] 只看 HTTP 状态码
来源：http://ojb.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ern.yangfankeji.com

[R61] 磁盘占用
来源：http://ihw.zhoulong.xyz

df -h;  du -sh *
来源：http://ywl.yongpay.top

[R62] 找最占空间的文件
来源：http://bbp.pengpengdd.cyou

du -ah . | sort -rh | head -10
来源：http://sna.daria6918.cn

[R63] 内存与进程
来源：http://jef.jianghu66.top

free -h;  ps aux | grep nginx
来源：http://gfy.zhiwuduotai.top

[R64] 结束进程
来源：http://fme.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://vus.ydjk.org.cn

[R65] 查看端口占用
来源：http://jhs.hongshengwenyu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xjr.xuetiantiany.cn

[R66] 定时任务
来源：http://adf.jinqigfzy.top

crontab -e;  crontab -l
来源：http://xwu.feifeiyinyue.top

[R67] 生成随机十六进制串
来源：http://cop.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://gac.aizwys.cn

[R68] 计算文件校验值
来源：http://yyk.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qpm.zdbjq.cn

[R69] 生成随机密码
来源：http://srh.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://fhh.sxryk.cn

[R70] 时间戳与互转
来源：http://qsi.jlsjyb.cn

date +%s;  date -d @1700000000
来源：http://vpp.pengpengdd.cyou

[R71] 日期格式化
来源：http://bpn.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://cux.hnxiangtu.top

[R72] 等待端口就绪
来源：http://jep.xingfuxueyuan.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://oig.zhaomingkeji.xyz

[R73] 分割大日志
来源：http://mjv.yj20258.top

split -l 1000 big.log part_
来源：http://aax.aizwys.cn

[R74] 批量重命名
来源：http://oja.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zpo.mhx1999.top

[R75] 导出环境变量
来源：http://uny.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://zhg.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://ggh.birdmap.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ehw.daria6918.cn

[R77] 读取用户输入
来源：http://kfu.sjlbkw.cn

read -rp "请输入: " ans
来源：http://kba.yuanzhike.top

[R78] 交互式菜单
来源：http://vzt.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xqo.vqdsnc.cn

[R79] 解析命令行选项
来源：http://rza.ybcxt.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mzc.yanxiufei.cn

[R80] 查看脚本执行耗时
来源：http://edk.zhaomingkeji.xyz

time ./run.sh
来源：http://uvz.jyoumei.cn

================================================================================
来源：http://tvp.yuanzhike.top

S. C / C++ 专题
来源：http://ayd.yj20258888.top

================================================================================
来源：http://hlf.zdbjq.cn

[S01] C：Hello World
来源：http://spa.fktsv.cn

#include <stdio.h>
来源：http://rpl.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bdk.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://msk.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://soi.zhongyouzk.top

[S03] C：读入整数
来源：http://arx.xziqi.cn

int x; scanf("%d", &x);
来源：http://uee.xylfe.cn

[S04] C：字符串复制
来源：http://ojl.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://anq.316326.xyz

[S05] C：字符串长度
来源：http://prh.yj20258.top

strlen(s)
来源：http://mkh.9152youxi.cn

[S06] C：字符串比较
来源：http://piw.nanxuanxn.top

strcmp(a, b) == 0
来源：http://mzj.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://wgt.jlsjyb.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oxk.yj20258.top

[S08] C：动态内存分配与释放
来源：http://pba.nanxinkj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cai.ydjk.org.cn

[S09] C：结构体定义与初始化
来源：http://kwa.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hzm.aibaodan.cn

[S10] C：指针与解引用
来源：http://dgp.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://prq.zhongyouzk.top

[S11] C：逐行读文件
来源：http://wud.tian-w.cn

FILE *f = fopen("a.txt", "r");
来源：http://wib.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://iqw.cucudq.cn

fclose(f);
来源：http://aok.guannengcc.top

[S12] C：写文件
来源：http://ufv.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ucy.kuanghao11.cn

[S13] C：宏定义
来源：http://lrx.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://usz.xziqi.cn

[S14] C：枚举
来源：http://apl.zhongyouzk.top

enum Color { RED, GREEN, BLUE };
来源：http://vrt.birdmap.top

[S15] C：类型转换
来源：http://hpr.jqgufenzy.top

(double) a / b
来源：http://jem.havefunace.top

[S16] C：位操作置位
来源：http://cvz.daria6918.cn

x |= (1 << 3);
来源：http://tbr.daxiang520.top

[S17] C：安全拼接字符串
来源：http://gpw.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eex.smart0.xyz

[S18] C：命令行参数
来源：http://wgb.guowangkeji.top

int main(int argc, char **argv)
来源：http://rwh.xziqi.cn

[S19] C：快速排序
来源：http://ocj.jinyuanbaomall.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uge.ivvv.top

[S20] C：二分查找
来源：http://kzr.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gfq.havefunace.top

[S21] C：字符类别判断
来源：http://tlo.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dba.jqgufenzy.top

[S22] C：字符串转数字
来源：http://lij.guannengcc.top


<!-- 参考信息 -->