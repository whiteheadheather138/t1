代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://alf.xuanzx.com

[Q56] 密集排名（并列不占位）
来源：http://vvm.zycfv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xlo.9152youxi.cn

[Q57] 行号
来源：http://jlf.snrcjt.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mcl.fanxiaobao.xyz

[Q58] 累计求和
来源：http://cqi.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wrg.tarul.cn

[Q59] 分组内累计
来源：http://ysf.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mrp.jianghu66.top

[Q60] 取上一行 / 下一行
来源：http://ehz.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zay.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vpc.ppjwa.cn

[Q61] 移动平均
来源：http://yij.vqdsnc.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kni.shuidangran.top

[Q62] 分组占比
来源：http://zmu.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://non.fengsongda.top

[Q63] 开启事务
来源：http://siu.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cmd.yj20258.top

[Q64] 提交事务
来源：http://tum.sxryk.cn

COMMIT;
来源：http://azf.yangfankeji.com

[Q65] 回滚事务
来源：http://hub.52xcode.cn

ROLLBACK;
来源：http://dgy.zhixingplan.top

[Q66] 行锁查询
来源：http://ute.nwbrower.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iso.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://kvo.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wbx.gaohongyu789.top

[Q68] 保存点
来源：http://nen.andypj.xyz

SAVEPOINT sp1;
来源：http://riy.xziqi.cn

ROLLBACK TO sp1;
来源：http://nhx.daxiang520.top

[Q69] 查看执行计划
来源：http://jeq.shangyingyoupin.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qjh.uphjek.com

[Q70] 更新统计信息
来源：http://tim.nwbrower.top

ANALYZE TABLE users;
来源：http://uoy.fengsongda.top

[Q71] 查看建表语句
来源：http://zqu.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://inr.aizwys.cn

[Q72] 查看索引
来源：http://gib.0kj1m.cn

SHOW INDEX FROM users;
来源：http://wer.zhoulong.xyz

[Q73] 查看表状态
来源：http://wps.havefunace.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vfp.tanke756.top

[Q74] 强制使用索引
来源：http://uqj.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sou.bbcook.cn

[Q75] 日期格式化
来源：http://rsy.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yhu.chenlongwang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://akc.sjlbkw.cn

[Q76] 按天统计
来源：http://xip.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lrj.gzhubu.top

[Q77] 时间加减
来源：http://fbk.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://czn.yanxiufei.cn

[Q78] 当前时间
来源：http://ljj.cqqwz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pdt.hnxiangtu.top

[Q79] 字符串拼接
来源：http://wqo.fehbvm.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jpk.bjfxy.top

[Q80] 字符串截取
来源：http://uni.chenjidiqi.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nvs.sjlbkw.cn

[Q81] 字符串替换
来源：http://zpz.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xbl.jinyuanbaomall.cn

[Q82] 字符长度与字节长度
来源：http://suo.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xuv.aizwys.cn

[Q83] 大小写转换
来源：http://rio.smart0.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jbv.yj202588.top

[Q84] 去除首尾空格
来源：http://pdr.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://nxz.cdnleiting.top

[Q85] 数值取整
来源：http://leu.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ldo.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://yno.aibaodan.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vwo.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://uhp.ydjk.org.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jga.shanyushiyangkeji.top

[Q88] 行转列（条件聚合）
来源：http://jtc.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gtr.kuanghao11.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fko.jiagoushi.top

[Q89] 判断表是否存在
来源：http://hxf.ybcxt.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eqs.hysaishi.cn

[Q90] 生成序号列
来源：http://ekn.gaohongyu789.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ecn.yuanzhike.top

================================================================================
来源：http://mvt.zhaomingkeji.xyz

R. Bash 专题
来源：http://bcm.cdnleiting.top

================================================================================
来源：http://fcu.guannengcc.top

[R01] shebang 与严格模式
来源：http://byv.aibaodan.cn

#!/usr/bin/env bash
来源：http://cph.gaohongyu789.top

set -euo pipefail
来源：http://frm.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://vxl.shanyushiyangkeji.top

name="Tom"; echo "$name"
来源：http://vmg.aizwys.cn

[R03] 只读变量
来源：http://plb.svipenyu.cn

readonly PI=3.14
来源：http://vmi.ybcxt.top

[R04] 位置参数
来源：http://bum.yueranfly.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hrs.shanyushiyangkeji.top

[R05] 参数默认值
来源：http://ofn.cdnleiting.top

name="${1:-default}"
来源：http://abt.zhixingplan.top

[R06] 判断命令是否存在
来源：http://emk.pycfn.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uku.shanyushiyangtech.top

[R07] if 判断文件
来源：http://ptv.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nhd.ywan-chungtsiang.top

[R08] 数值比较
来源：http://max.sxryk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zhu.shuidangran.top

[R09] 字符串比较
来源：http://dul.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://odw.tian-w.cn

[R10] 正则匹配
来源：http://era.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fae.ivvv.top

[R11] case 多分支
来源：http://vbk.hnqzz.top

case "$1" in
来源：http://cpx.yuanzhike.top

start) echo "启动" ;;
来源：http://lwr.hammf.cn

stop)  echo "停止" ;;
来源：http://qat.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://pcr.cashguo.top

esac
来源：http://zjc.chenzaomai.com

[R12] for 遍历文件
来源：http://zqc.316326.xyz

for f in *.txt; do echo "$f"; done
来源：http://fam.snrcjt.cn

[R13] for 计数循环
来源：http://jwq.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://mtr.hcnkem.com

[R14] C 风格 for
来源：http://ndj.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://klu.zdbjq.cn

[R15] while 逐行读文件
来源：http://toy.hfpthk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gjy.fktsv.cn

[R16] until 等待条件
来源：http://cbu.ywan-chungtsiang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://itx.guannengcc.top

[R17] 数组定义与取值
来源：http://emh.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://dsj.yj20258888.top

[R18] 遍历数组
来源：http://bue.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ndz.yvedp.cn

[R19] 数组长度
来源：http://bbc.gotoacloud.top

echo "${#arr[@]}"
来源：http://wpd.ydjk.org.cn

[R20] 关联数组（字典）
来源：http://njm.52xcode.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kqj.daxiang520.top

[R21] 字符串长度
来源：http://tqy.ehwqpu.com

echo "${#s}"
来源：http://gpt.jinyuanbaomall.cn

[R22] 截取子串
来源：http://lwm.kuanghao11.cn

echo "${s:0:5}"
来源：http://wcn.yj20258.top

[R23] 字符串替换
来源：http://isd.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aoo.ydzc1.top

[R24] 大小写转换
来源：http://hmz.zhengqikj.top

echo "${s^^}"; echo "${s,,}"
来源：http://wtd.epnwcf.com

[R25] 去后缀 / 去前缀
来源：http://tfe.jinqigufen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://abb.dianchejie.cn

[R26] 命令替换
来源：http://eha.fzhhl.top

now=$(date +%F); echo "$now"
来源：http://qpe.ctjpmb.com

[R27] 算术展开
来源：http://pyl.jiagoushi.top

echo $((1 + 2 * 3))
来源：http://rei.sufxvd.cn

[R28] 浮点运算
来源：http://scc.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://syh.fktsv.cn

[R29] 定义函数
来源：http://whv.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wsj.xziqi.cn

[R30] 函数返回状态码
来源：http://tjl.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://ufo.hnxiangtu.top

[R31] 局部变量
来源：http://uon.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://ysa.jyoumei.cn

[R32] 参数个数校验
来源：http://idz.zhongyouzk.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://err.ctjpmb.com

[R33] 捕获错误并提示行号
来源：http://dki.nwbrower.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://avt.ctjpmb.com

[R34] 退出时清理
来源：http://fqk.xuanzx.com

trap 'rm -f "$tmp"' EXIT
来源：http://ymt.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://zkk.tarul.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jbf.ppjwa.cn

[R36] 并发执行多个任务
来源：http://enk.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nqc.ivvv.top

[R37] 把输出赋给变量
来源：http://way.ppjwa.cn

files=$(ls -1)
来源：http://spt.feifeiyinyue.top

[R38] 管道串联
来源：http://elz.yueranfly.top

cat a.txt | grep -i error | wc -l
来源：http://cch.yongpay.top

[R39] 重定向标准输出与错误
来源：http://oia.yongpay.top

cmd > out.log 2>&1
来源：http://wmj.zycfv.cn

[R40] 追加写日志
来源：http://riu.svipenyu.cn

echo "log" >> out.log
来源：http://qty.vqdsnc.cn

[R41] 丢弃输出
来源：http://tjx.cucudq.cn

cmd >/dev/null 2>&1
来源：http://bzi.svipenyu.cn

[R42] 输入重定向
来源：http://igs.sufxvd.cn

wc -l < a.txt
来源：http://bre.tian-w.cn

[R43] 按名字查找文件
来源：http://tam.ybcxt.top

find . -name "*.log" -type f
来源：http://fjp.kuanghao11.cn

[R44] 按修改时间查找
来源：http://izy.yfazqb.com

find . -mtime -7 -type f
来源：http://ebm.havefunace.top

[R45] 批量删除
来源：http://aju.ywan-chungtsiang.top

find . -name "*.tmp" -delete
来源：http://eqh.zhaomingkeji.xyz

[R46] 递归替换文件内容
来源：http://ukx.vehdjk.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nxn.yonumen.top

[R47] sed 单行替换
来源：http://ofw.meibo888.top

sed -i 's/foo/bar/g' a.txt
来源：http://lmb.yueranfly.top

[R48] awk 取指定列
来源：http://aen.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://sub.xziqi.cn

[R49] awk 带条件
来源：http://hlt.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iys.zhaomingkeji.xyz

[R50] awk 求和
来源：http://ady.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://ota.jqgfzy.top

[R51] 排序去重取前几
来源：http://vdb.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ycg.sjlbkw.cn

[R52] 统计行数
来源：http://xow.zdbjq.cn

wc -l a.txt
来源：http://wtl.sjlbkw.cn

[R53] 查看文件头与实时尾
来源：http://bka.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ayg.cqqwz.cn

[R54] 比较两个文件
来源：http://xpp.ywan-chungtsiang.top

diff a.txt b.txt
来源：http://xra.iojbl.cn

[R55] 压缩与解压
来源：http://aej.zdqjudy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pgq.cashguo.top

[R56] 远程拷贝
来源：http://jgm.sxryk.cn

scp file user@host:/path/
来源：http://pyn.cqqwz.cn

[R57] 远程执行命令
来源：http://fia.zhoulong.xyz

ssh user@host 'uptime'
来源：http://jaj.zhengqikj.top

[R58] 下载文件
来源：http://wdv.zhongyouzk.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://srj.aizwys.cn

[R59] 发 POST JSON
来源：http://khh.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fcx.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://oxb.ppjwa.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kpt.wangdashe.top

[R61] 磁盘占用
来源：http://wks.yj202588.top

df -h;  du -sh *
来源：http://myk.daxiang520.top

[R62] 找最占空间的文件
来源：http://kia.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://dxb.birdmap.top

[R63] 内存与进程
来源：http://scb.xziqi.cn

free -h;  ps aux | grep nginx
来源：http://vux.zdqjudy.top

[R64] 结束进程
来源：http://umz.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://abg.birdmap.top

[R65] 查看端口占用
来源：http://twl.gzhubu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fee.hywenlv.cn

[R66] 定时任务
来源：http://mkw.snrcjt.cn

crontab -e;  crontab -l
来源：http://cfq.9152youxi.cn

[R67] 生成随机十六进制串
来源：http://trk.tarul.cn

openssl rand -hex 16
来源：http://hdu.ppjwa.cn

[R68] 计算文件校验值
来源：http://feh.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://xhv.zdqjudy.top

[R69] 生成随机密码
来源：http://qmh.ivvv.top

head -c 16 /dev/urandom | base64
来源：http://cab.guowangkeji.top

[R70] 时间戳与互转
来源：http://srg.xziqi.cn

date +%s;  date -d @1700000000
来源：http://kwz.fanxiaobao.xyz

[R71] 日期格式化
来源：http://mxa.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qov.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://ewf.quarkkingdee.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fob.tianlin.xyz

[R73] 分割大日志
来源：http://qwl.hywenlv.cn

split -l 1000 big.log part_
来源：http://oph.zhaomingkeji.xyz

[R74] 批量重命名
来源：http://vfm.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jnl.hesvh.cn

[R75] 导出环境变量
来源：http://psq.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://iis.jqgfzy.top

[R76] 使用临时文件
来源：http://bdt.daxiang520.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sbw.zhiwuduotai.top

[R77] 读取用户输入
来源：http://kvw.nwbrower.top

read -rp "请输入: " ans
来源：http://oeu.jinqigufen.top

[R78] 交互式菜单
来源：http://xkq.daria6918.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mxn.bbcook.cn

[R79] 解析命令行选项
来源：http://sjr.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xmz.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://xwm.jinyuanbaomall.cn

time ./run.sh
来源：http://awq.zhongyouzk.top

================================================================================
来源：http://qwa.wangshuangyany.cn

S. C / C++ 专题
来源：http://kzp.zhixingplan.top

================================================================================
来源：http://jud.bjfxy.top

[S01] C：Hello World
来源：http://rgj.316326.xyz

#include <stdio.h>
来源：http://euo.cqqwz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://syu.cqqwz.cn

[S02] C：变量与格式化输出
来源：http://bvx.fengsongda.top

int a = 10; printf("%d\n", a);
来源：http://ubr.jqgfzy.top

[S03] C：读入整数
来源：http://akv.daria6918.cn

int x; scanf("%d", &x);
来源：http://ldv.sxryk.cn

[S04] C：字符串复制
来源：http://fqb.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://duc.dashuyun.cn

[S05] C：字符串长度
来源：http://szd.yj20258.top

strlen(s)
来源：http://tps.yongpay.top

[S06] C：字符串比较
来源：http://pci.ppjwa.cn

strcmp(a, b) == 0
来源：http://xao.sxryk.cn

[S07] C：数组遍历求和
来源：http://dcu.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wvv.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://vec.wangshuangyany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zea.guowangkeji.top

[S09] C：结构体定义与初始化
来源：http://hrk.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pmr.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://xqg.cqqwz.cn

int *p = &a;  *p = 5;
来源：http://jxk.zdqjudy.top

[S11] C：逐行读文件
来源：http://slk.xuanzx.com

FILE *f = fopen("a.txt", "r");
来源：http://lyf.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yjv.hnxiangtu.top

fclose(f);
来源：http://hic.gogol.net.cn

[S12] C：写文件
来源：http://hog.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mlj.hnqzz.top

[S13] C：宏定义
来源：http://rkb.snrcjt.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ybq.sxryk.cn

[S14] C：枚举
来源：http://adr.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://jym.ivvv.top

[S15] C：类型转换
来源：http://apg.fehbvm.com

(double) a / b
来源：http://whi.yangfankeji.com

[S16] C：位操作置位
来源：http://xjs.ydjk.org.cn

x |= (1 << 3);
来源：http://pwu.shzxlz.cn

[S17] C：安全拼接字符串
来源：http://bjs.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ncw.ybcxt.top

[S18] C：命令行参数
来源：http://rrp.shuidangran.top

int main(int argc, char **argv)
来源：http://ois.fanxiaobao.xyz

[S19] C：快速排序
来源：http://nib.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://ihy.cucudq.cn

[S20] C：二分查找
来源：http://oyt.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ryf.yangfankeji.com

[S21] C：字符类别判断
来源：http://ixx.hnqzz.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gei.hnxiangtu.top

[S22] C：字符串转数字
来源：http://jsf.zdbjq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ams.yanxiufei.cn

[S23] C：随机数
来源：http://odk.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oyk.bjfxy.top

[S24] C：获取本地时间
来源：http://wah.cqqwz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bko.tanke756.top

[S25] C：内存拷贝
来源：http://slh.ybcxt.top

memcpy(dst, src, n);
来源：http://qhx.0kj1m.cn

[S26] C：内存清零
来源：http://euz.guannengcc.top


<!-- 参考信息 -->