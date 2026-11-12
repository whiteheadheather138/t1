代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gqg.kuanghao11.cn

[Q58] 累计求和
来源：http://kqu.tianlin.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nmh.sjlbkw.cn

[Q59] 分组内累计
来源：http://qmc.gaohongyu789.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hoc.haohaochexian.top

[Q60] 取上一行 / 下一行
来源：http://klm.nanxinkj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wqw.uphjek.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qat.dashuyun.cn

[Q61] 移动平均
来源：http://gfs.ctjpmb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wdw.vqdsnc.cn

[Q62] 分组占比
来源：http://xey.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wvr.guowangkeji.top

[Q63] 开启事务
来源：http://gig.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://csf.yj202588.top

[Q64] 提交事务
来源：http://uwn.bbcook.cn

COMMIT;
来源：http://qmt.chenzaomai.com

[Q65] 回滚事务
来源：http://dun.quarkkingdee.top

ROLLBACK;
来源：http://ycu.jyoumei.cn

[Q66] 行锁查询
来源：http://tdy.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ohh.zhoulong.xyz

[Q67] 设置隔离级别
来源：http://gds.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rtd.jyoumei.cn

[Q68] 保存点
来源：http://izp.sxryk.cn

SAVEPOINT sp1;
来源：http://ayl.bbcook.cn

ROLLBACK TO sp1;
来源：http://svx.andypj.xyz

[Q69] 查看执行计划
来源：http://mxg.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pmj.yj20258888.top

[Q70] 更新统计信息
来源：http://idp.jqgufenzy.top

ANALYZE TABLE users;
来源：http://rnk.ydjk.org.cn

[Q71] 查看建表语句
来源：http://whc.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dxa.xinyue.icu

[Q72] 查看索引
来源：http://dgk.gogol.net.cn

SHOW INDEX FROM users;
来源：http://jri.aibaodan.cn

[Q73] 查看表状态
来源：http://pxb.birdmap.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kko.pengpengdd.cyou

[Q74] 强制使用索引
来源：http://zos.pengpengdd.cyou

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://svl.redwolf501.top

[Q75] 日期格式化
来源：http://ouc.zhaomingkeji.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zol.vehdjk.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gpb.yj202588.top

[Q76] 按天统计
来源：http://yyv.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vgx.hnxiangtu.top

[Q77] 时间加减
来源：http://xzy.vqdsnc.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yse.ywan-chungtsiang.top

[Q78] 当前时间
来源：http://bnc.vehdjk.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dpq.jqgfzy.top

[Q79] 字符串拼接
来源：http://euq.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://okj.zhengqikj.top

[Q80] 字符串截取
来源：http://xqh.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oic.shangyingyoupin.top

[Q81] 字符串替换
来源：http://ppk.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ndx.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://lhu.chenjidiqi.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pss.yj202588.top

[Q83] 大小写转换
来源：http://mje.hysaishi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dfb.hcnkem.com

[Q84] 去除首尾空格
来源：http://ndd.jinqigufen.top

SELECT TRIM(name) FROM users;
来源：http://yqb.tian-w.cn

[Q85] 数值取整
来源：http://qoa.ppjwa.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gxs.wangdashe.top

[Q86] 读取 JSON 字段
来源：http://nff.gaohongyu789.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vva.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://tlo.cqqwz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pfe.hfpthk.cn

[Q88] 行转列（条件聚合）
来源：http://mgp.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dtm.52xcode.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qpi.316326.xyz

[Q89] 判断表是否存在
来源：http://ysj.snrcjt.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vqp.daxiang520.top

[Q90] 生成序号列
来源：http://olu.tianlin.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tyg.aizwys.cn

================================================================================
来源：http://dyz.xuetiantiany.cn

R. Bash 专题
来源：http://gkp.meibo888.top

================================================================================
来源：http://pgb.guannengcc.top

[R01] shebang 与严格模式
来源：http://vwt.hesvh.cn

#!/usr/bin/env bash
来源：http://pyw.havefunace.top

set -euo pipefail
来源：http://pen.chenlongwang.top

[R02] 变量赋值与使用
来源：http://ekm.zdbjq.cn

name="Tom"; echo "$name"
来源：http://pcd.shanyushiyangtech.top

[R03] 只读变量
来源：http://wol.ywan-chungtsiang.top

readonly PI=3.14
来源：http://qvd.jiagoushi.top

[R04] 位置参数
来源：http://soq.aizwys.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dfo.ivvv.top

[R05] 参数默认值
来源：http://xrq.yj20258.top

name="${1:-default}"
来源：http://zlp.zhongyouzk.top

[R06] 判断命令是否存在
来源：http://alp.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wbd.fengsongda.top

[R07] if 判断文件
来源：http://xwj.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mkw.aizwys.cn

[R08] 数值比较
来源：http://dec.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://din.quarkkingdee.top

[R09] 字符串比较
来源：http://qvd.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ghq.dashuyun.cn

[R10] 正则匹配
来源：http://xvp.sysykeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mkd.yuanzhike.top

[R11] case 多分支
来源：http://czp.smart0.xyz

case "$1" in
来源：http://ezf.pengpengdd.cyou

start) echo "启动" ;;
来源：http://ysl.guowangkeji.top

stop)  echo "停止" ;;
来源：http://lfe.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://iif.xylfe.cn

esac
来源：http://ahp.hywenlv.cn

[R12] for 遍历文件
来源：http://blh.yj20258888.top

for f in *.txt; do echo "$f"; done
来源：http://mmx.hnxiangtu.top

[R13] for 计数循环
来源：http://koy.hongshengwenyu.top

for i in {1..10}; do echo "$i"; done
来源：http://bnq.feifeiyinyue.top

[R14] C 风格 for
来源：http://ggu.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yyq.cdnleiting.top

[R15] while 逐行读文件
来源：http://nqz.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nvw.redwolf501.top

[R16] until 等待条件
来源：http://tvg.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zzu.aizwys.cn

[R17] 数组定义与取值
来源：http://kct.sjlbkw.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tzh.tian-w.cn

[R18] 遍历数组
来源：http://ggp.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ilh.haohaochexian.top

[R19] 数组长度
来源：http://nhb.yfazqb.com

echo "${#arr[@]}"
来源：http://krv.sweek.top

[R20] 关联数组（字典）
来源：http://vah.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cxu.pengpengdd.cyou

[R21] 字符串长度
来源：http://wux.havefunace.top

echo "${#s}"
来源：http://pbl.yj20258888.top

[R22] 截取子串
来源：http://meb.nwbrower.top

echo "${s:0:5}"
来源：http://mji.jinqigufen.top

[R23] 字符串替换
来源：http://epf.jlsjyb.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hnh.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://uvg.52xcode.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gll.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://fwt.yueranfly.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://khy.svipenyu.cn

[R26] 命令替换
来源：http://sus.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://txz.tianlin.xyz

[R27] 算术展开
来源：http://ial.nanxuanxn.top

echo $((1 + 2 * 3))
来源：http://ack.cdnleiting.top

[R28] 浮点运算
来源：http://uki.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://txp.ehwqpu.com

[R29] 定义函数
来源：http://bfd.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cdr.fzhhl.top

[R30] 函数返回状态码
来源：http://lut.xuanzx.com

f() { return 0; }; f || echo "失败了"
来源：http://xsg.aizwys.cn

[R31] 局部变量
来源：http://gpo.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://kkf.smart0.xyz

[R32] 参数个数校验
来源：http://oxg.tarul.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yih.tanke756.top

[R33] 捕获错误并提示行号
来源：http://don.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fkh.guannengcc.top

[R34] 退出时清理
来源：http://wko.gogol.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ihr.jinghuilouyu.cn

[R35] 后台执行并等待
来源：http://udi.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://dne.xuetiantiany.cn

[R36] 并发执行多个任务
来源：http://llf.zhixingplan.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dqy.yongpay.top

[R37] 把输出赋给变量
来源：http://kux.gzhubu.top

files=$(ls -1)
来源：http://imb.xylfe.cn

[R38] 管道串联
来源：http://lmz.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://dvg.yj20258888.top

[R39] 重定向标准输出与错误
来源：http://mje.smart0.xyz

cmd > out.log 2>&1
来源：http://esw.zhoulong.xyz

[R40] 追加写日志
来源：http://bmv.yj20258.top

echo "log" >> out.log
来源：http://mtn.cqqwz.cn

[R41] 丢弃输出
来源：http://zul.daria6918.cn

cmd >/dev/null 2>&1
来源：http://ljf.jqgufenzy.top

[R42] 输入重定向
来源：http://zbm.gzhubu.top

wc -l < a.txt
来源：http://dng.daxiang520.top

[R43] 按名字查找文件
来源：http://abc.hywenlv.cn

find . -name "*.log" -type f
来源：http://eva.jyoumei.cn

[R44] 按修改时间查找
来源：http://wpw.guowangkeji.top

find . -mtime -7 -type f
来源：http://vso.bbcook.cn

[R45] 批量删除
来源：http://exs.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://fdt.jyoumei.cn

[R46] 递归替换文件内容
来源：http://bjh.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dhy.yj202588.top

[R47] sed 单行替换
来源：http://krv.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://gba.zhijiandao.cn

[R48] awk 取指定列
来源：http://fpj.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://zeu.yj20258888.top

[R49] awk 带条件
来源：http://nfx.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qti.jqgufenzy.top

[R50] awk 求和
来源：http://ine.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rro.zhengqikj.top

[R51] 排序去重取前几
来源：http://wff.zhiwuduotai.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qto.wangshuangyany.cn

[R52] 统计行数
来源：http://mgw.yueranfly.top

wc -l a.txt
来源：http://xan.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://tcs.jinghuilouyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ynq.yj20258.top

[R54] 比较两个文件
来源：http://bhs.hammf.cn

diff a.txt b.txt
来源：http://uuc.nanxuanxn.top

[R55] 压缩与解压
来源：http://kdg.aibaodan.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ijo.quarkkingdee.top

[R56] 远程拷贝
来源：http://mvk.guannengcc.top

scp file user@host:/path/
来源：http://ztz.jyoumei.cn

[R57] 远程执行命令
来源：http://ohx.ehwqpu.com

ssh user@host 'uptime'
来源：http://crc.jiagoushi.top

[R58] 下载文件
来源：http://xrj.redwolf501.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lki.hnxiangtu.top

[R59] 发 POST JSON
来源：http://kim.c1oappe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fkp.epnwcf.com

[R60] 只看 HTTP 状态码
来源：http://uvy.wangshuangyany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pyv.dashuyun.cn

[R61] 磁盘占用
来源：http://qah.hesvh.cn

df -h;  du -sh *
来源：http://khy.zdbjq.cn

[R62] 找最占空间的文件
来源：http://rak.316326.xyz

du -ah . | sort -rh | head -10
来源：http://ivn.iojbl.cn

[R63] 内存与进程
来源：http://sni.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://xsw.fanxiaobao.xyz

[R64] 结束进程
来源：http://lgt.hammf.cn

kill -9 $(pgrep -f app.py)
来源：http://mev.hammf.cn

[R65] 查看端口占用
来源：http://dwy.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gdl.nwbrower.top

[R66] 定时任务
来源：http://tut.jyoumei.cn

crontab -e;  crontab -l
来源：http://gzp.jlsjyb.cn

[R67] 生成随机十六进制串
来源：http://voa.fanxiaobao.xyz

openssl rand -hex 16
来源：http://lpj.hammf.cn

[R68] 计算文件校验值
来源：http://noo.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iaz.yfazqb.com

[R69] 生成随机密码
来源：http://qwl.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://rfk.yj202588.top

[R70] 时间戳与互转
来源：http://nxa.hcnkem.com

date +%s;  date -d @1700000000
来源：http://nrm.zhaomingkeji.xyz

[R71] 日期格式化
来源：http://vqi.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fwl.bbcook.cn

[R72] 等待端口就绪
来源：http://lvx.316326.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://sie.snrcjt.cn

[R73] 分割大日志
来源：http://npb.jinyuanbaomall.cn

split -l 1000 big.log part_
来源：http://wtp.iojbl.cn

[R74] 批量重命名
来源：http://nqw.uphjek.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://prt.cucudq.cn

[R75] 导出环境变量
来源：http://asy.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://cnv.shzxlz.cn

[R76] 使用临时文件
来源：http://vxb.haohaochexian.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bsy.nanxinkj.top

[R77] 读取用户输入
来源：http://bmi.cdnleiting.top

read -rp "请输入: " ans
来源：http://rdl.sxryk.cn

[R78] 交互式菜单
来源：http://ikt.kuanghao11.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gdb.cucudq.cn

[R79] 解析命令行选项
来源：http://nno.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xfn.c1oappe.top

[R80] 查看脚本执行耗时
来源：http://zsm.hongshengwenyu.top

time ./run.sh
来源：http://qtb.tian-w.cn

================================================================================
来源：http://cpy.yueranfly.top

S. C / C++ 专题
来源：http://kit.chenlongwang.top

================================================================================
来源：http://syp.dashuyun.cn

[S01] C：Hello World
来源：http://fwv.quarkkingdee.top

#include <stdio.h>
来源：http://vep.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bwq.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://kby.shanyushiyangtech.top

int a = 10; printf("%d\n", a);
来源：http://bfi.c1oappe.top

[S03] C：读入整数
来源：http://mea.zhixingplan.top

int x; scanf("%d", &x);
来源：http://xfv.0kj1m.cn

[S04] C：字符串复制
来源：http://gvp.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uue.aizwys.cn

[S05] C：字符串长度
来源：http://yrz.gotoacloud.top

strlen(s)
来源：http://awo.wangdashe.top

[S06] C：字符串比较
来源：http://teb.uphjek.com

strcmp(a, b) == 0
来源：http://nex.tianlin.xyz

[S07] C：数组遍历求和
来源：http://lpl.tarul.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kbx.yj20258888.top

[S08] C：动态内存分配与释放
来源：http://cjw.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uko.feifeiyinyue.top

[S09] C：结构体定义与初始化
来源：http://mja.chenzaomai.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dsv.nanxuanxn.top

[S10] C：指针与解引用
来源：http://can.redwolf501.top

int *p = &a;  *p = 5;
来源：http://wgw.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://ifq.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://qpg.jqgufenzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kdd.nanxinkj.top

fclose(f);
来源：http://vib.yj202588.top

[S12] C：写文件
来源：http://rxy.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jcc.hysaishi.cn

[S13] C：宏定义
来源：http://jnj.cdnleiting.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lpo.ybcxt.top

[S14] C：枚举
来源：http://mjf.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://cbp.hcnkem.com

[S15] C：类型转换
来源：http://mjb.nanxuanxn.top

(double) a / b
来源：http://spn.epnwcf.com

[S16] C：位操作置位
来源：http://rbg.yj202588.top

x |= (1 << 3);
来源：http://xsi.iojbl.cn

[S17] C：安全拼接字符串
来源：http://ahd.zycfv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cik.fktsv.cn

[S18] C：命令行参数
来源：http://bcs.epnwcf.com

int main(int argc, char **argv)
来源：http://yvl.aibaodan.cn

[S19] C：快速排序
来源：http://qyu.yj20258.top

qsort(a, n, sizeof(int), cmp);
来源：http://cte.ppjwa.cn

[S20] C：二分查找
来源：http://lqu.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ayo.xziqi.cn

[S21] C：字符类别判断
来源：http://fnb.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hdu.yj20258888.top

[S22] C：字符串转数字
来源：http://jxl.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://nhj.hcnkem.com

[S23] C：随机数
来源：http://mwt.guannengcc.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mpg.redwolf501.top

[S24] C：获取本地时间
来源：http://gwh.zdbjq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://emc.haohaochexian.top

[S25] C：内存拷贝
来源：http://kfn.yvedp.cn

memcpy(dst, src, n);
来源：http://cij.sweek.top

[S26] C：内存清零
来源：http://aru.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://stj.daria6918.cn

[S27] C：定义常量
来源：http://cgo.yuanzhike.top

const double PI = 3.14159;
来源：http://wgs.zhixingplan.top

[S28] C：静态变量
来源：http://viz.aibaodan.cn


<!-- 参考信息 -->