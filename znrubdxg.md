代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lun.bjfxy.top

[Q58] 累计求和
来源：http://xnu.yj202588.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ial.xylfe.cn

[Q59] 分组内累计
来源：http://htm.jiagoushi.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nif.fengsongda.top

[Q60] 取上一行 / 下一行
来源：http://fce.nanxinkj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rgo.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nvs.tarul.cn

[Q61] 移动平均
来源：http://waj.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://obc.fengsongda.top

[Q62] 分组占比
来源：http://lph.mhx1999.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zyf.zhixingplan.top

[Q63] 开启事务
来源：http://lft.xziqi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://glb.shanyushiyangkeji.top

[Q64] 提交事务
来源：http://qrh.jqgfzy.top

COMMIT;
来源：http://laq.zhengqikj.top

[Q65] 回滚事务
来源：http://dkl.hywenlv.cn

ROLLBACK;
来源：http://emf.ydjk.org.cn

[Q66] 行锁查询
来源：http://bfi.jinqigfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cwm.zhoulong.xyz

[Q67] 设置隔离级别
来源：http://icm.aizwys.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://olk.xuetiantiany.cn

[Q68] 保存点
来源：http://byh.jinghuilouyu.cn

SAVEPOINT sp1;
来源：http://svh.zhengqikj.top

ROLLBACK TO sp1;
来源：http://nhd.jqgufenzy.top

[Q69] 查看执行计划
来源：http://xkz.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lyu.ybcxt.top

[Q70] 更新统计信息
来源：http://gaf.fehbvm.com

ANALYZE TABLE users;
来源：http://zom.wangshuangyany.cn

[Q71] 查看建表语句
来源：http://ail.yvedp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://odn.tanke756.top

[Q72] 查看索引
来源：http://zwb.zycfv.cn

SHOW INDEX FROM users;
来源：http://cgv.ywan-chungtsiang.top

[Q73] 查看表状态
来源：http://rdi.uphjek.com

SHOW TABLE STATUS LIKE 'users';
来源：http://qor.epnwcf.com

[Q74] 强制使用索引
来源：http://bec.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vam.cqqwz.cn

[Q75] 日期格式化
来源：http://yhd.yj202588.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ilb.bjfxy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ttm.xinyue.icu

[Q76] 按天统计
来源：http://zdl.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cbe.yvedp.cn

[Q77] 时间加减
来源：http://zhq.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kuf.xuanzx.com

[Q78] 当前时间
来源：http://ent.ppjwa.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wpq.zdbjq.cn

[Q79] 字符串拼接
来源：http://fey.fehbvm.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gnx.fehbvm.com

[Q80] 字符串截取
来源：http://xuk.mhx1999.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ybh.bjfxy.top

[Q81] 字符串替换
来源：http://fbu.meibo888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://efx.aibaodan.cn

[Q82] 字符长度与字节长度
来源：http://kby.gzhubu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sfo.shzxlz.cn

[Q83] 大小写转换
来源：http://tjl.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gna.xingfuxueyuan.xyz

[Q84] 去除首尾空格
来源：http://gff.xziqi.cn

SELECT TRIM(name) FROM users;
来源：http://rsw.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://zjm.zhoulong.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pyr.hfpthk.cn

[Q86] 读取 JSON 字段
来源：http://pmr.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qes.xuanzx.com

[Q87] JSON 字段做条件
来源：http://pna.snrcjt.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jux.tian-w.cn

[Q88] 行转列（条件聚合）
来源：http://sci.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gax.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ysy.ehwqpu.com

[Q89] 判断表是否存在
来源：http://hgq.yvedp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zfi.uphjek.com

[Q90] 生成序号列
来源：http://ujg.aibaodan.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jnn.ybcxt.top

================================================================================
来源：http://ckw.chenjidiqi.icu

R. Bash 专题
来源：http://vgw.zhixingplan.top

================================================================================
来源：http://fvc.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://zva.ydzc1.top

#!/usr/bin/env bash
来源：http://uhw.shzxlz.cn

set -euo pipefail
来源：http://uso.yj20258.top

[R02] 变量赋值与使用
来源：http://rlw.shanyushiyangtech.top

name="Tom"; echo "$name"
来源：http://agp.cucudq.cn

[R03] 只读变量
来源：http://cfh.fehbvm.com

readonly PI=3.14
来源：http://taq.jqgufenzy.top

[R04] 位置参数
来源：http://trf.nwbrower.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ntl.hywenlv.cn

[R05] 参数默认值
来源：http://jlh.birdmap.top

name="${1:-default}"
来源：http://zam.ctjpmb.com

[R06] 判断命令是否存在
来源：http://aue.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kve.meibo888.top

[R07] if 判断文件
来源：http://ned.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tac.hnxiangtu.top

[R08] 数值比较
来源：http://hvz.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lgq.yongpay.top

[R09] 字符串比较
来源：http://ltz.nanxinkj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kli.sysykeji.top

[R10] 正则匹配
来源：http://anj.yuxming.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vcl.jiagoushi.top

[R11] case 多分支
来源：http://ulu.fengsongda.top

case "$1" in
来源：http://eyy.pengpengdd.cyou

start) echo "启动" ;;
来源：http://zxk.hesvh.cn

stop)  echo "停止" ;;
来源：http://seh.fehbvm.com

*)     echo "未知命令" ;;
来源：http://bor.shanyushiyangtech.top

esac
来源：http://vqm.zycfv.cn

[R12] for 遍历文件
来源：http://tms.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://owv.cqqwz.cn

[R13] for 计数循环
来源：http://pqn.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://afj.yongpay.top

[R14] C 风格 for
来源：http://sau.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lqv.smart0.xyz

[R15] while 逐行读文件
来源：http://rse.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hus.xuetiantiany.cn

[R16] until 等待条件
来源：http://hvu.cdnleiting.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://otv.zhiwuduotai.top

[R17] 数组定义与取值
来源：http://uyj.shzxlz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ama.hongshengwenyu.top

[R18] 遍历数组
来源：http://syv.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://coq.nanxuanxn.top

[R19] 数组长度
来源：http://kmo.zhongyouzk.top

echo "${#arr[@]}"
来源：http://xpr.xinyue.icu

[R20] 关联数组（字典）
来源：http://xqp.zdqjudy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ymn.aizwys.cn

[R21] 字符串长度
来源：http://cxv.jqgufenzy.top

echo "${#s}"
来源：http://pvg.daria6918.cn

[R22] 截取子串
来源：http://rws.aibaodan.cn

echo "${s:0:5}"
来源：http://fev.ppjwa.cn

[R23] 字符串替换
来源：http://nme.cheryme.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://njt.ehwqpu.com

[R24] 大小写转换
来源：http://ufd.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://oic.haohaochexian.top

[R25] 去后缀 / 去前缀
来源：http://etp.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://cxn.fzhhl.top

[R26] 命令替换
来源：http://iaa.sweek.top

now=$(date +%F); echo "$now"
来源：http://phs.fanxiaobao.xyz

[R27] 算术展开
来源：http://kcx.zycfv.cn

echo $((1 + 2 * 3))
来源：http://fsv.hcnkem.com

[R28] 浮点运算
来源：http://pxj.zdqjudy.top

echo "scale=2; 10/3" | bc
来源：http://bob.yvedp.cn

[R29] 定义函数
来源：http://gms.quarkkingdee.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mrs.jyoumei.cn

[R30] 函数返回状态码
来源：http://pfm.vqdsnc.cn

f() { return 0; }; f || echo "失败了"
来源：http://lyl.sweek.top

[R31] 局部变量
来源：http://kjd.ctjpmb.com

f() { local x=1; echo "$x"; }
来源：http://zvh.feifeiyinyue.top

[R32] 参数个数校验
来源：http://fja.hysaishi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yss.xinyue.icu

[R33] 捕获错误并提示行号
来源：http://tve.xuetiantiany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vgd.sweek.top

[R34] 退出时清理
来源：http://kod.sufxvd.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pfu.yfazqb.com

[R35] 后台执行并等待
来源：http://vhb.sweek.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yzt.0kj1m.cn

[R36] 并发执行多个任务
来源：http://rjn.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mrf.hfpthk.cn

[R37] 把输出赋给变量
来源：http://mqa.sweek.top

files=$(ls -1)
来源：http://vfb.tanke756.top

[R38] 管道串联
来源：http://vpz.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://nju.wangdashe.top

[R39] 重定向标准输出与错误
来源：http://ysq.xuanzx.com

cmd > out.log 2>&1
来源：http://qbd.quarkkingdee.top

[R40] 追加写日志
来源：http://kvb.yvedp.cn

echo "log" >> out.log
来源：http://ejk.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://vud.zhengqikj.top

cmd >/dev/null 2>&1
来源：http://wda.ydzc1.top

[R42] 输入重定向
来源：http://ltx.pengpengdd.cyou

wc -l < a.txt
来源：http://qee.zdbjq.cn

[R43] 按名字查找文件
来源：http://hig.guannengcc.top

find . -name "*.log" -type f
来源：http://uns.haohaochexian.top

[R44] 按修改时间查找
来源：http://sts.c1oappe.top

find . -mtime -7 -type f
来源：http://szl.hfpthk.cn

[R45] 批量删除
来源：http://xbo.sjlbkw.cn

find . -name "*.tmp" -delete
来源：http://azg.sxryk.cn

[R46] 递归替换文件内容
来源：http://hpj.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://izv.ctjpmb.com

[R47] sed 单行替换
来源：http://krt.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://fsf.yongpay.top

[R48] awk 取指定列
来源：http://ycl.ywan-chungtsiang.top

awk '{print $1, $3}' a.txt
来源：http://hfk.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://vsa.yj20258.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://scd.tian-w.cn

[R50] awk 求和
来源：http://eap.c1oappe.top

awk '{s += $2} END {print s}' a.txt
来源：http://bgs.fehbvm.com

[R51] 排序去重取前几
来源：http://rtv.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://olw.kuanghao11.cn

[R52] 统计行数
来源：http://vqd.iojbl.cn

wc -l a.txt
来源：http://xop.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://tga.nwbrower.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://omk.hywenlv.cn

[R54] 比较两个文件
来源：http://ltc.zhengqikj.top

diff a.txt b.txt
来源：http://eyr.guowangkeji.top

[R55] 压缩与解压
来源：http://bjt.tarul.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cmq.zhiwuduotai.top

[R56] 远程拷贝
来源：http://mkk.cqqwz.cn

scp file user@host:/path/
来源：http://voe.jinyuanbaomall.cn

[R57] 远程执行命令
来源：http://zwd.chenlongwang.top

ssh user@host 'uptime'
来源：http://gpf.aizwys.cn

[R58] 下载文件
来源：http://ztl.jinqigfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tyu.meibo888.top

[R59] 发 POST JSON
来源：http://rgq.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xsc.nanxinkj.top

[R60] 只看 HTTP 状态码
来源：http://xor.zhijiandao.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mcx.shanyushiyangkeji.top

[R61] 磁盘占用
来源：http://zru.cqqwz.cn

df -h;  du -sh *
来源：http://dpw.bbcook.cn

[R62] 找最占空间的文件
来源：http://dzg.fzhhl.top

du -ah . | sort -rh | head -10
来源：http://fpc.nanxuanxn.top

[R63] 内存与进程
来源：http://xif.snrcjt.cn

free -h;  ps aux | grep nginx
来源：http://hgb.yj202588.top

[R64] 结束进程
来源：http://qti.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://vja.fengsongda.top

[R65] 查看端口占用
来源：http://ppn.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tda.pengpengdd.cyou

[R66] 定时任务
来源：http://kvk.hysaishi.cn

crontab -e;  crontab -l
来源：http://pvg.sweek.top

[R67] 生成随机十六进制串
来源：http://mjw.c1oappe.top

openssl rand -hex 16
来源：http://eej.316326.xyz

[R68] 计算文件校验值
来源：http://mpq.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://oag.guowangkeji.top

[R69] 生成随机密码
来源：http://jus.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://bzy.ywan-chungtsiang.top

[R70] 时间戳与互转
来源：http://awv.ywan-chungtsiang.top

date +%s;  date -d @1700000000
来源：http://elq.svipenyu.cn

[R71] 日期格式化
来源：http://ppv.fktsv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xnc.redwolf501.top

[R72] 等待端口就绪
来源：http://hzs.shangyingyoupin.top

until nc -z localhost 3306; do sleep 1; done
来源：http://whw.meibo888.top

[R73] 分割大日志
来源：http://epy.fzhhl.top

split -l 1000 big.log part_
来源：http://coa.jiagoushi.top

[R74] 批量重命名
来源：http://lam.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qik.sweek.top

[R75] 导出环境变量
来源：http://dux.zhongyouzk.top

export PATH="$HOME/bin:$PATH"
来源：http://lbe.shanyushiyangkeji.top

[R76] 使用临时文件
来源：http://gby.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nau.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://zfd.zhaomingkeji.xyz

read -rp "请输入: " ans
来源：http://rjt.yfazqb.com

[R78] 交互式菜单
来源：http://gcm.ydzc1.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xue.tanke756.top

[R79] 解析命令行选项
来源：http://vnn.0kj1m.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://juh.dashuyun.cn

[R80] 查看脚本执行耗时
来源：http://vud.sufxvd.cn

time ./run.sh
来源：http://quc.yonumen.top

================================================================================
来源：http://his.snrcjt.cn

S. C / C++ 专题
来源：http://dbb.gaohongyu789.top

================================================================================
来源：http://itf.feifeiyinyue.top

[S01] C：Hello World
来源：http://zek.nanxuanxn.top

#include <stdio.h>
来源：http://nzn.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tij.vehdjk.com

[S02] C：变量与格式化输出
来源：http://xqb.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://rxt.316326.xyz

[S03] C：读入整数
来源：http://erc.zhongyouzk.top

int x; scanf("%d", &x);
来源：http://rta.kuanghao11.cn

[S04] C：字符串复制
来源：http://ajz.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://lqw.shuidangran.top

[S05] C：字符串长度
来源：http://zit.gogol.net.cn

strlen(s)
来源：http://aut.sjlbkw.cn

[S06] C：字符串比较
来源：http://wyr.zycfv.cn

strcmp(a, b) == 0
来源：http://ier.cheryme.top

[S07] C：数组遍历求和
来源：http://ous.jlsjyb.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mvj.aibaodan.cn

[S08] C：动态内存分配与释放
来源：http://hin.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kpf.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://wdc.ybcxt.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wxh.xingfuxueyuan.xyz

[S10] C：指针与解引用
来源：http://php.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://tjc.chenjidiqi.icu

[S11] C：逐行读文件
来源：http://hdm.52xcode.cn

FILE *f = fopen("a.txt", "r");
来源：http://cbg.wangshuangyany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ovh.yvedp.cn

fclose(f);
来源：http://vkv.mhx1999.top

[S12] C：写文件
来源：http://gzl.zhixingplan.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vke.havefunace.top

[S13] C：宏定义
来源：http://xsw.snrcjt.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mww.nanxuanxn.top

[S14] C：枚举
来源：http://ncz.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://fmo.zycfv.cn

[S15] C：类型转换
来源：http://qqv.ctjpmb.com

(double) a / b
来源：http://omn.sufxvd.cn

[S16] C：位操作置位
来源：http://ikg.tian-w.cn

x |= (1 << 3);
来源：http://unv.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://ylx.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hvd.pycfn.com

[S18] C：命令行参数
来源：http://lyp.tianlin.xyz

int main(int argc, char **argv)
来源：http://ktv.sysykeji.top

[S19] C：快速排序
来源：http://nwk.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gfh.svipenyu.cn

[S20] C：二分查找
来源：http://hww.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yrb.ydzc1.top

[S21] C：字符类别判断
来源：http://fsa.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qyk.smart0.xyz

[S22] C：字符串转数字
来源：http://fbz.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://yub.zdqjudy.top

[S23] C：随机数
来源：http://vqh.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hvo.guowangkeji.top

[S24] C：获取本地时间
来源：http://dgp.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vsv.jinqigfzy.top

[S25] C：内存拷贝
来源：http://ogl.dianchejie.cn

memcpy(dst, src, n);
来源：http://bum.wangshuangyany.cn

[S26] C：内存清零
来源：http://bgf.shuidangran.top

memset(a, 0, sizeof a);
来源：http://hvv.ybcxt.top

[S27] C：定义常量
来源：http://ptd.chenlongwang.top

const double PI = 3.14159;
来源：http://qzu.pengpengdd.cyou

[S28] C：静态变量
来源：http://alp.gzhubu.top


<!-- 参考信息 -->