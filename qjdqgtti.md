代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xec.kuanghao11.cn

[Q58] 累计求和
来源：http://dli.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iyd.52xcode.cn

[Q59] 分组内累计
来源：http://lwu.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://job.cdnleiting.top

[Q60] 取上一行 / 下一行
来源：http://khn.gotoacloud.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cnp.9152youxi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sqc.wangdashe.top

[Q61] 移动平均
来源：http://fed.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mfk.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://rxi.fengsongda.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pzy.jinqigufen.top

[Q63] 开启事务
来源：http://dnj.hammf.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uge.cashguo.top

[Q64] 提交事务
来源：http://fhr.snrcjt.cn

COMMIT;
来源：http://tpd.ywan-chungtsiang.top

[Q65] 回滚事务
来源：http://dxu.jqgfzy.top

ROLLBACK;
来源：http://pma.haohaochexian.top

[Q66] 行锁查询
来源：http://vsc.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ywh.svipenyu.cn

[Q67] 设置隔离级别
来源：http://vtz.sweek.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hox.smart0.xyz

[Q68] 保存点
来源：http://ttw.epnwcf.com

SAVEPOINT sp1;
来源：http://tfb.quarkkingdee.top

ROLLBACK TO sp1;
来源：http://bri.guannengcc.top

[Q69] 查看执行计划
来源：http://luc.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tur.aizwys.cn

[Q70] 更新统计信息
来源：http://who.yj202588.top

ANALYZE TABLE users;
来源：http://kld.meibo888.top

[Q71] 查看建表语句
来源：http://kcp.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ten.yongpay.top

[Q72] 查看索引
来源：http://jrn.ctjpmb.com

SHOW INDEX FROM users;
来源：http://mia.jinqigfzy.top

[Q73] 查看表状态
来源：http://rks.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yys.xingfuxueyuan.xyz

[Q74] 强制使用索引
来源：http://hit.jianghu66.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qxa.jinyuanbaomall.cn

[Q75] 日期格式化
来源：http://fme.shanyushiyangtech.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ict.snrcjt.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uas.cucudq.cn

[Q76] 按天统计
来源：http://wqy.shuidangran.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://usa.jinqigfzy.top

[Q77] 时间加减
来源：http://wzz.feifeiyinyue.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yhk.nanxinkj.top

[Q78] 当前时间
来源：http://mgt.shanyushiyangtech.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gmo.zhijiandao.cn

[Q79] 字符串拼接
来源：http://bjv.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qup.pengpengdd.cyou

[Q80] 字符串截取
来源：http://vvz.pengpengdd.cyou

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xnd.vqdsnc.cn

[Q81] 字符串替换
来源：http://tli.birdmap.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xjq.dianchejie.cn

[Q82] 字符长度与字节长度
来源：http://toq.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hpc.xinyue.icu

[Q83] 大小写转换
来源：http://egn.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qeq.zdqjudy.top

[Q84] 去除首尾空格
来源：http://llm.sweek.top

SELECT TRIM(name) FROM users;
来源：http://qec.bjfxy.top

[Q85] 数值取整
来源：http://jzc.xingfuxueyuan.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ayr.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://nof.fengsongda.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qzt.ehwqpu.com

[Q87] JSON 字段做条件
来源：http://qju.hywenlv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gco.uphjek.com

[Q88] 行转列（条件聚合）
来源：http://tge.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qez.nwbrower.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sde.guowangkeji.top

[Q89] 判断表是否存在
来源：http://vcf.xylfe.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hkc.zhengqikj.top

[Q90] 生成序号列
来源：http://xol.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vbq.xziqi.cn

================================================================================
来源：http://dcz.sysykeji.top

R. Bash 专题
来源：http://krt.hnxiangtu.top

================================================================================
来源：http://wof.cucudq.cn

[R01] shebang 与严格模式
来源：http://agc.zhengqikj.top

#!/usr/bin/env bash
来源：http://szd.ehwqpu.com

set -euo pipefail
来源：http://srj.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://qea.yonumen.top

name="Tom"; echo "$name"
来源：http://tja.yongpay.top

[R03] 只读变量
来源：http://lpd.cdnleiting.top

readonly PI=3.14
来源：http://ecj.hywenlv.cn

[R04] 位置参数
来源：http://iyj.jyoumei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bsd.snrcjt.cn

[R05] 参数默认值
来源：http://erm.zhixingplan.top

name="${1:-default}"
来源：http://wni.nanxuanxn.top

[R06] 判断命令是否存在
来源：http://man.ydzc1.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dmz.cdnleiting.top

[R07] if 判断文件
来源：http://sar.hnqzz.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iep.cdnleiting.top

[R08] 数值比较
来源：http://boh.zhiwuduotai.top

if (( a > b )); then echo "a 更大"; fi
来源：http://kbi.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://vtv.jinyuanbaomall.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gtn.smart0.xyz

[R10] 正则匹配
来源：http://and.jinghuilouyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://utl.daxiang520.top

[R11] case 多分支
来源：http://rcj.zhijiandao.cn

case "$1" in
来源：http://gmz.cqqwz.cn

start) echo "启动" ;;
来源：http://doo.aizwys.cn

stop)  echo "停止" ;;
来源：http://qjz.bbcook.cn

*)     echo "未知命令" ;;
来源：http://kln.wangshuangyany.cn

esac
来源：http://vav.tanke756.top

[R12] for 遍历文件
来源：http://mie.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://poi.ywan-chungtsiang.top

[R13] for 计数循环
来源：http://elu.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://ixy.shuidangran.top

[R14] C 风格 for
来源：http://vko.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bsc.yj20258888.top

[R15] while 逐行读文件
来源：http://rhl.cashguo.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jmm.yuanzhike.top

[R16] until 等待条件
来源：http://uau.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mwi.zhoulong.xyz

[R17] 数组定义与取值
来源：http://qnn.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://nbi.nanxuanxn.top

[R18] 遍历数组
来源：http://iec.xuanzx.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kct.yueranfly.top

[R19] 数组长度
来源：http://rpi.guannengcc.top

echo "${#arr[@]}"
来源：http://eln.kuanghao11.cn

[R20] 关联数组（字典）
来源：http://eew.yvedp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kcz.sufxvd.cn

[R21] 字符串长度
来源：http://rbw.xuanzx.com

echo "${#s}"
来源：http://yjx.kuanghao11.cn

[R22] 截取子串
来源：http://ofp.hcnkem.com

echo "${s:0:5}"
来源：http://dtg.bjfxy.top

[R23] 字符串替换
来源：http://epo.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hxm.hfpthk.cn

[R24] 大小写转换
来源：http://sdd.mhx1999.top

echo "${s^^}"; echo "${s,,}"
来源：http://qjm.xingfuxueyuan.xyz

[R25] 去后缀 / 去前缀
来源：http://zji.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://woo.jlsjyb.cn

[R26] 命令替换
来源：http://fzs.sweek.top

now=$(date +%F); echo "$now"
来源：http://ctd.yangfankeji.com

[R27] 算术展开
来源：http://zal.jlsjyb.cn

echo $((1 + 2 * 3))
来源：http://tca.uphjek.com

[R28] 浮点运算
来源：http://fii.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://scm.hcnkem.com

[R29] 定义函数
来源：http://iwh.ydjk.org.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wyd.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://tsg.shanyushiyangtech.top

f() { return 0; }; f || echo "失败了"
来源：http://mcs.shanyushiyangtech.top

[R31] 局部变量
来源：http://ecs.jianghu66.top

f() { local x=1; echo "$x"; }
来源：http://slm.ydjk.org.cn

[R32] 参数个数校验
来源：http://sqb.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ezd.yuanzhike.top

[R33] 捕获错误并提示行号
来源：http://tpt.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://toe.yuanzhike.top

[R34] 退出时清理
来源：http://wac.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qya.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://jcb.hnqzz.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xad.shzxlz.cn

[R36] 并发执行多个任务
来源：http://tpj.vqdsnc.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tyg.tarul.cn

[R37] 把输出赋给变量
来源：http://dhq.nwbrower.top

files=$(ls -1)
来源：http://eut.gotoacloud.top

[R38] 管道串联
来源：http://zst.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://waw.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://byq.nwbrower.top

cmd > out.log 2>&1
来源：http://rvz.yueranfly.top

[R40] 追加写日志
来源：http://yti.shangyingyoupin.top

echo "log" >> out.log
来源：http://fih.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://ctz.fehbvm.com

cmd >/dev/null 2>&1
来源：http://uen.havefunace.top

[R42] 输入重定向
来源：http://rsh.dianchejie.cn

wc -l < a.txt
来源：http://kbq.yj202588.top

[R43] 按名字查找文件
来源：http://vgr.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://ipn.tarul.cn

[R44] 按修改时间查找
来源：http://lva.zdbjq.cn

find . -mtime -7 -type f
来源：http://sot.hnxiangtu.top

[R45] 批量删除
来源：http://hrf.gaohongyu789.top

find . -name "*.tmp" -delete
来源：http://zrw.kuanghao11.cn

[R46] 递归替换文件内容
来源：http://ujj.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xjf.ctjpmb.com

[R47] sed 单行替换
来源：http://csz.yanxiufei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bwo.hfpthk.cn

[R48] awk 取指定列
来源：http://bls.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://vad.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://yzt.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://chd.mhx1999.top

[R50] awk 求和
来源：http://qww.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://avj.redwolf501.top

[R51] 排序去重取前几
来源：http://inb.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cbh.cqqwz.cn

[R52] 统计行数
来源：http://sut.hywenlv.cn

wc -l a.txt
来源：http://zsb.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://det.fehbvm.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qbs.jlsjyb.cn

[R54] 比较两个文件
来源：http://urh.guannengcc.top

diff a.txt b.txt
来源：http://anl.fanxiaobao.xyz

[R55] 压缩与解压
来源：http://qry.sjlbkw.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lfc.gaohongyu789.top

[R56] 远程拷贝
来源：http://gxd.zhaomingkeji.xyz

scp file user@host:/path/
来源：http://rrp.redwolf501.top

[R57] 远程执行命令
来源：http://zlj.smart0.xyz

ssh user@host 'uptime'
来源：http://pgo.redwolf501.top

[R58] 下载文件
来源：http://txv.aizwys.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://twb.fktsv.cn

[R59] 发 POST JSON
来源：http://bzl.mhx1999.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://utk.sjlbkw.cn

[R60] 只看 HTTP 状态码
来源：http://ogt.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pfa.jianghu66.top

[R61] 磁盘占用
来源：http://bjl.tianlin.xyz

df -h;  du -sh *
来源：http://iqu.iojbl.cn

[R62] 找最占空间的文件
来源：http://tzq.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://brh.yj20258.top

[R63] 内存与进程
来源：http://tyg.hongshengwenyu.top

free -h;  ps aux | grep nginx
来源：http://bxl.haohaochexian.top

[R64] 结束进程
来源：http://oqi.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://tsj.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://awa.cdnleiting.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://edg.bjfxy.top

[R66] 定时任务
来源：http://aqj.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://lav.bjfxy.top

[R67] 生成随机十六进制串
来源：http://yqv.yuxming.cn

openssl rand -hex 16
来源：http://aas.ybcxt.top

[R68] 计算文件校验值
来源：http://nqk.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://dpu.aibaodan.cn

[R69] 生成随机密码
来源：http://ban.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://rcz.cdnleiting.top

[R70] 时间戳与互转
来源：http://azk.tarul.cn

date +%s;  date -d @1700000000
来源：http://qiq.sxryk.cn

[R71] 日期格式化
来源：http://tat.gzhubu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mku.shzxlz.cn

[R72] 等待端口就绪
来源：http://mol.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cxi.ivvv.top

[R73] 分割大日志
来源：http://fnq.cdnleiting.top

split -l 1000 big.log part_
来源：http://gis.shzxlz.cn

[R74] 批量重命名
来源：http://iaf.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://idi.yueranfly.top

[R75] 导出环境变量
来源：http://qca.smart0.xyz

export PATH="$HOME/bin:$PATH"
来源：http://vly.yuanzhike.top

[R76] 使用临时文件
来源：http://twa.svipenyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fvf.jianghu66.top

[R77] 读取用户输入
来源：http://fti.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://itb.hysaishi.cn

[R78] 交互式菜单
来源：http://jdo.cucudq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hae.ydzc1.top

[R79] 解析命令行选项
来源：http://mhd.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rag.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://mbf.aibaodan.cn

time ./run.sh
来源：http://qzy.zhoulong.xyz

================================================================================
来源：http://ypt.zhoulong.xyz

S. C / C++ 专题
来源：http://dpx.sjlbkw.cn

================================================================================
来源：http://dyl.daxiang520.top

[S01] C：Hello World
来源：http://bep.guannengcc.top

#include <stdio.h>
来源：http://njz.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://sir.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://ffh.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://qsm.shzxlz.cn

[S03] C：读入整数
来源：http://xrk.havefunace.top

int x; scanf("%d", &x);
来源：http://yky.gogol.net.cn

[S04] C：字符串复制
来源：http://elu.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://lit.jinyuanbaomall.cn

[S05] C：字符串长度
来源：http://zkl.tarul.cn

strlen(s)
来源：http://cth.quarkkingdee.top

[S06] C：字符串比较
来源：http://frh.dianchejie.cn

strcmp(a, b) == 0
来源：http://wtt.zhiwuduotai.top

[S07] C：数组遍历求和
来源：http://mdl.ybcxt.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yzv.havefunace.top

[S08] C：动态内存分配与释放
来源：http://nuf.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bbi.yueranfly.top

[S09] C：结构体定义与初始化
来源：http://gwx.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://joj.yj20258888.top

[S10] C：指针与解引用
来源：http://ght.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://xpx.haohaochexian.top

[S11] C：逐行读文件
来源：http://eyk.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://zuw.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hpi.yuanzhike.top

fclose(f);
来源：http://xho.c1oappe.top

[S12] C：写文件
来源：http://sde.52xcode.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pxg.andypj.xyz

[S13] C：宏定义
来源：http://bmz.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lce.xuanzx.com

[S14] C：枚举
来源：http://mzf.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://grx.ydzc1.top

[S15] C：类型转换
来源：http://xic.jinghuilouyu.cn

(double) a / b
来源：http://wjg.smart0.xyz

[S16] C：位操作置位
来源：http://cnp.xuanzx.com

x |= (1 << 3);
来源：http://ldk.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://sqf.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://upr.sjlbkw.cn

[S18] C：命令行参数
来源：http://cdl.gogol.net.cn

int main(int argc, char **argv)
来源：http://wzr.dianchejie.cn

[S19] C：快速排序
来源：http://fzi.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iwq.dianchejie.cn

[S20] C：二分查找
来源：http://cuy.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jvt.shzxlz.cn

[S21] C：字符类别判断
来源：http://fow.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dfo.sjlbkw.cn

[S22] C：字符串转数字
来源：http://eua.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pur.smart0.xyz

[S23] C：随机数
来源：http://vda.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wgy.chenlongwang.top

[S24] C：获取本地时间
来源：http://gns.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xtd.birdmap.top

[S25] C：内存拷贝
来源：http://hks.gotoacloud.top

memcpy(dst, src, n);
来源：http://syq.daxiang520.top

[S26] C：内存清零
来源：http://mxj.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://yzx.mhx1999.top

[S27] C：定义常量
来源：http://asb.jiagoushi.top

const double PI = 3.14159;
来源：http://efe.xingfuxueyuan.xyz

[S28] C：静态变量
来源：http://akg.fengsongda.top


<!-- 参考信息 -->