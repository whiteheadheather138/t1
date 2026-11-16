代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cwv.yanxiufei.cn

[Q58] 累计求和
来源：http://wpm.316326.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://svz.sweek.top

[Q59] 分组内累计
来源：http://pve.nwbrower.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cyq.yongpay.top

[Q60] 取上一行 / 下一行
来源：http://emw.nanxuanxn.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nnv.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mje.jqgufenzy.top

[Q61] 移动平均
来源：http://ipw.zdqjudy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gvg.tanke756.top

[Q62] 分组占比
来源：http://kqi.yj202588.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wqc.hywenlv.cn

[Q63] 开启事务
来源：http://ojs.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cbx.vehdjk.com

[Q64] 提交事务
来源：http://mzj.ppjwa.cn

COMMIT;
来源：http://hyx.yfazqb.com

[Q65] 回滚事务
来源：http://rfz.hnxiangtu.top

ROLLBACK;
来源：http://mgo.gzhubu.top

[Q66] 行锁查询
来源：http://rwu.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iqh.316326.xyz

[Q67] 设置隔离级别
来源：http://bpl.fzhhl.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yvt.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://jsu.dashuyun.cn

SAVEPOINT sp1;
来源：http://dwb.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://rak.andypj.xyz

[Q69] 查看执行计划
来源：http://kmh.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wqv.chenjidiqi.icu

[Q70] 更新统计信息
来源：http://fqn.pycfn.com

ANALYZE TABLE users;
来源：http://ags.nwbrower.top

[Q71] 查看建表语句
来源：http://cxx.gogol.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cyd.xinyue.icu

[Q72] 查看索引
来源：http://ijd.dianchejie.cn

SHOW INDEX FROM users;
来源：http://ctf.jqgfzy.top

[Q73] 查看表状态
来源：http://tum.zycfv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pdd.daxiang520.top

[Q74] 强制使用索引
来源：http://zpe.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kmd.zhengqikj.top

[Q75] 日期格式化
来源：http://mob.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ake.sufxvd.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vxk.guowangkeji.top

[Q76] 按天统计
来源：http://tyt.fzhhl.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gns.sweek.top

[Q77] 时间加减
来源：http://vzw.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mkz.tanke756.top

[Q78] 当前时间
来源：http://nhb.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cqa.tianlin.xyz

[Q79] 字符串拼接
来源：http://naw.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cnt.yj20258.top

[Q80] 字符串截取
来源：http://ljc.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iyj.jiagoushi.top

[Q81] 字符串替换
来源：http://riy.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ktr.zhiwuduotai.top

[Q82] 字符长度与字节长度
来源：http://aml.gotoacloud.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://chd.xuetiantiany.cn

[Q83] 大小写转换
来源：http://fgn.zhixingplan.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bis.daria6918.cn

[Q84] 去除首尾空格
来源：http://fpd.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://ptn.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://nyk.jinqigfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://asd.dashuyun.cn

[Q86] 读取 JSON 字段
来源：http://bxx.jianghu66.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ddx.hnxiangtu.top

[Q87] JSON 字段做条件
来源：http://aup.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wug.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://lay.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kuc.shzxlz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bna.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://hpc.ivvv.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kzq.jiagoushi.top

[Q90] 生成序号列
来源：http://qvv.gogol.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ven.shzxlz.cn

================================================================================
来源：http://ttc.jiagoushi.top

R. Bash 专题
来源：http://huf.hfpthk.cn

================================================================================
来源：http://exo.andypj.xyz

[R01] shebang 与严格模式
来源：http://xtz.iojbl.cn

#!/usr/bin/env bash
来源：http://llt.jyoumei.cn

set -euo pipefail
来源：http://ueb.nanxinkj.top

[R02] 变量赋值与使用
来源：http://pxb.meibo888.top

name="Tom"; echo "$name"
来源：http://ago.ydzc1.top

[R03] 只读变量
来源：http://gag.fzhhl.top

readonly PI=3.14
来源：http://jna.sxryk.cn

[R04] 位置参数
来源：http://ods.zhongyouzk.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wuv.sweek.top

[R05] 参数默认值
来源：http://hpl.jlsjyb.cn

name="${1:-default}"
来源：http://kag.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://tiy.ydzc1.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zds.cdnleiting.top

[R07] if 判断文件
来源：http://ukl.zhijiandao.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wri.shzxlz.cn

[R08] 数值比较
来源：http://meb.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nig.nanxinkj.top

[R09] 字符串比较
来源：http://tpg.vehdjk.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ect.hysaishi.cn

[R10] 正则匹配
来源：http://ynx.yvedp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://euk.cashguo.top

[R11] case 多分支
来源：http://ftz.zycfv.cn

case "$1" in
来源：http://yth.pycfn.com

start) echo "启动" ;;
来源：http://cgs.zdbjq.cn

stop)  echo "停止" ;;
来源：http://ktc.yongpay.top

*)     echo "未知命令" ;;
来源：http://lhv.zhongyouzk.top

esac
来源：http://tkd.hywenlv.cn

[R12] for 遍历文件
来源：http://tiv.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://djd.yuxming.cn

[R13] for 计数循环
来源：http://vgc.yj202588.top

for i in {1..10}; do echo "$i"; done
来源：http://ntj.gzhubu.top

[R14] C 风格 for
来源：http://qkh.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bvu.ivvv.top

[R15] while 逐行读文件
来源：http://jrt.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://atp.yonumen.top

[R16] until 等待条件
来源：http://kwe.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://quy.gotoacloud.top

[R17] 数组定义与取值
来源：http://vfv.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://hlr.cashguo.top

[R18] 遍历数组
来源：http://toi.aibaodan.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://grp.vqdsnc.cn

[R19] 数组长度
来源：http://aud.shzxlz.cn

echo "${#arr[@]}"
来源：http://kbq.hfpthk.cn

[R20] 关联数组（字典）
来源：http://xpv.dianchejie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zgz.yuanzhike.top

[R21] 字符串长度
来源：http://mxl.chenzaomai.com

echo "${#s}"
来源：http://mgo.gotoacloud.top

[R22] 截取子串
来源：http://vix.chenjidiqi.icu

echo "${s:0:5}"
来源：http://guf.uphjek.com

[R23] 字符串替换
来源：http://ghe.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://efe.nanxuanxn.top

[R24] 大小写转换
来源：http://gab.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nnt.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://btd.yj20258888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oyn.daria6918.cn

[R26] 命令替换
来源：http://law.feifeiyinyue.top

now=$(date +%F); echo "$now"
来源：http://xnr.yangfankeji.com

[R27] 算术展开
来源：http://ptb.c1oappe.top

echo $((1 + 2 * 3))
来源：http://pep.zycfv.cn

[R28] 浮点运算
来源：http://vno.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://dig.aizwys.cn

[R29] 定义函数
来源：http://qyb.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gyk.ivvv.top

[R30] 函数返回状态码
来源：http://noj.hcnkem.com

f() { return 0; }; f || echo "失败了"
来源：http://hya.gogol.net.cn

[R31] 局部变量
来源：http://pjt.guowangkeji.top

f() { local x=1; echo "$x"; }
来源：http://xvs.svipenyu.cn

[R32] 参数个数校验
来源：http://xei.xylfe.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tix.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://kqh.havefunace.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sni.fengsongda.top

[R34] 退出时清理
来源：http://lea.hysaishi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zjg.bjfxy.top

[R35] 后台执行并等待
来源：http://wbq.sweek.top

sleep 5 & pid=$!; wait "$pid"
来源：http://cks.yueranfly.top

[R36] 并发执行多个任务
来源：http://hhs.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hob.dashuyun.cn

[R37] 把输出赋给变量
来源：http://hdl.tarul.cn

files=$(ls -1)
来源：http://uvt.shzxlz.cn

[R38] 管道串联
来源：http://vde.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://sui.ivvv.top

[R39] 重定向标准输出与错误
来源：http://idt.yuxming.cn

cmd > out.log 2>&1
来源：http://tls.xuetiantiany.cn

[R40] 追加写日志
来源：http://szg.bbcook.cn

echo "log" >> out.log
来源：http://wav.tarul.cn

[R41] 丢弃输出
来源：http://vhu.pycfn.com

cmd >/dev/null 2>&1
来源：http://yjw.zhengqikj.top

[R42] 输入重定向
来源：http://sct.hongshengwenyu.top

wc -l < a.txt
来源：http://lot.bbcook.cn

[R43] 按名字查找文件
来源：http://wvm.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://vjj.uphjek.com

[R44] 按修改时间查找
来源：http://yfs.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://mbm.tanke756.top

[R45] 批量删除
来源：http://cya.yj20258888.top

find . -name "*.tmp" -delete
来源：http://oxj.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://gmj.yongpay.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://psg.52xcode.cn

[R47] sed 单行替换
来源：http://ube.hnqzz.top

sed -i 's/foo/bar/g' a.txt
来源：http://zhm.hnqzz.top

[R48] awk 取指定列
来源：http://eja.kuanghao11.cn

awk '{print $1, $3}' a.txt
来源：http://alf.ctjpmb.com

[R49] awk 带条件
来源：http://sfw.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jmm.jiagoushi.top

[R50] awk 求和
来源：http://sul.hesvh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jhb.xuanzx.com

[R51] 排序去重取前几
来源：http://jsm.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mzw.hfpthk.cn

[R52] 统计行数
来源：http://ptp.jinyuanbaomall.cn

wc -l a.txt
来源：http://rwm.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://lun.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mbm.jyoumei.cn

[R54] 比较两个文件
来源：http://mfp.kuanghao11.cn

diff a.txt b.txt
来源：http://urh.kuanghao11.cn

[R55] 压缩与解压
来源：http://tnj.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ejg.bjfxy.top

[R56] 远程拷贝
来源：http://qya.chenlongwang.top

scp file user@host:/path/
来源：http://ebi.yuxming.cn

[R57] 远程执行命令
来源：http://obq.hfpthk.cn

ssh user@host 'uptime'
来源：http://bcw.svipenyu.cn

[R58] 下载文件
来源：http://lqk.kuanghao11.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ggm.redwolf501.top

[R59] 发 POST JSON
来源：http://pda.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pco.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://rlm.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zfj.sweek.top

[R61] 磁盘占用
来源：http://dnu.chenlongwang.top

df -h;  du -sh *
来源：http://kdq.tanke756.top

[R62] 找最占空间的文件
来源：http://ukk.tanke756.top

du -ah . | sort -rh | head -10
来源：http://muy.yj202588.top

[R63] 内存与进程
来源：http://qly.xylfe.cn

free -h;  ps aux | grep nginx
来源：http://mcg.fengsongda.top

[R64] 结束进程
来源：http://qmr.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://zaz.gzhubu.top

[R65] 查看端口占用
来源：http://iqg.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wua.nwbrower.top

[R66] 定时任务
来源：http://aut.zhixingplan.top

crontab -e;  crontab -l
来源：http://dte.yueranfly.top

[R67] 生成随机十六进制串
来源：http://hir.jinyuanbaomall.cn

openssl rand -hex 16
来源：http://nte.yj20258888.top

[R68] 计算文件校验值
来源：http://pbn.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://ptd.chenzaomai.com

[R69] 生成随机密码
来源：http://keh.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://jrc.yongpay.top

[R70] 时间戳与互转
来源：http://ntx.fanxiaobao.xyz

date +%s;  date -d @1700000000
来源：http://oir.dianchejie.cn

[R71] 日期格式化
来源：http://ijr.yj20258888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://spu.yangfankeji.com

[R72] 等待端口就绪
来源：http://xzk.zhaomingkeji.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://jlk.haohaochexian.top

[R73] 分割大日志
来源：http://ogy.tarul.cn

split -l 1000 big.log part_
来源：http://tgq.cqqwz.cn

[R74] 批量重命名
来源：http://czx.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mlj.jinyuanbaomall.cn

[R75] 导出环境变量
来源：http://ajq.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://rym.yanxiufei.cn

[R76] 使用临时文件
来源：http://xfu.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ftm.fktsv.cn

[R77] 读取用户输入
来源：http://non.zhoulong.xyz

read -rp "请输入: " ans
来源：http://saj.xinyue.icu

[R78] 交互式菜单
来源：http://trb.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://rik.mhx1999.top

[R79] 解析命令行选项
来源：http://oar.vehdjk.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qcx.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://wai.feifeiyinyue.top

time ./run.sh
来源：http://row.iojbl.cn

================================================================================
来源：http://wbj.iojbl.cn

S. C / C++ 专题
来源：http://mdp.shanyushiyangkeji.top

================================================================================
来源：http://olu.vqdsnc.cn

[S01] C：Hello World
来源：http://oyq.9152youxi.cn

#include <stdio.h>
来源：http://nwa.fehbvm.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://jga.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://bbj.jqgufenzy.top

int a = 10; printf("%d\n", a);
来源：http://anj.dashuyun.cn

[S03] C：读入整数
来源：http://awm.tianlin.xyz

int x; scanf("%d", &x);
来源：http://wjj.zhengqikj.top

[S04] C：字符串复制
来源：http://zzh.epnwcf.com

char dst[32]; strcpy(dst, "hi");
来源：http://fcf.fengsongda.top

[S05] C：字符串长度
来源：http://xvq.wangdashe.top

strlen(s)
来源：http://lqz.chenzaomai.com

[S06] C：字符串比较
来源：http://abs.zhixingplan.top

strcmp(a, b) == 0
来源：http://eld.fengsongda.top

[S07] C：数组遍历求和
来源：http://raa.nanxinkj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tty.hysaishi.cn

[S08] C：动态内存分配与释放
来源：http://auq.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lht.zdbjq.cn

[S09] C：结构体定义与初始化
来源：http://toe.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gks.birdmap.top

[S10] C：指针与解引用
来源：http://yqu.ydzc1.top

int *p = &a;  *p = 5;
来源：http://zpy.yanxiufei.cn

[S11] C：逐行读文件
来源：http://bxo.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://umr.jqgufenzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hxw.cheryme.top

fclose(f);
来源：http://cuk.xinyue.icu

[S12] C：写文件
来源：http://uwp.wangshuangyany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://npa.meibo888.top

[S13] C：宏定义
来源：http://ahm.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jzo.cashguo.top

[S14] C：枚举
来源：http://rhi.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://scf.tianlin.xyz

[S15] C：类型转换
来源：http://blz.zycfv.cn

(double) a / b
来源：http://nci.hfpthk.cn

[S16] C：位操作置位
来源：http://ctq.shuidangran.top

x |= (1 << 3);
来源：http://nky.jyoumei.cn

[S17] C：安全拼接字符串
来源：http://por.zdqjudy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tcg.hcnkem.com

[S18] C：命令行参数
来源：http://qvu.zhijiandao.cn

int main(int argc, char **argv)
来源：http://hzd.iojbl.cn

[S19] C：快速排序
来源：http://kcg.jianghu66.top

qsort(a, n, sizeof(int), cmp);
来源：http://dpg.daria6918.cn

[S20] C：二分查找
来源：http://juu.yvedp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rta.dianchejie.cn

[S21] C：字符类别判断
来源：http://tiu.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://otq.shangyingyoupin.top

[S22] C：字符串转数字
来源：http://mrx.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ptz.hesvh.cn

[S23] C：随机数
来源：http://bea.fktsv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lox.yangfankeji.com

[S24] C：获取本地时间
来源：http://izc.smart0.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hzc.jyoumei.cn

[S25] C：内存拷贝
来源：http://qkx.yj20258888.top

memcpy(dst, src, n);
来源：http://qnf.daxiang520.top

[S26] C：内存清零
来源：http://icr.chenlongwang.top

memset(a, 0, sizeof a);
来源：http://jdl.ydzc1.top

[S27] C：定义常量
来源：http://fhs.pengpengdd.cyou

const double PI = 3.14159;
来源：http://rqw.hnqzz.top

[S28] C：静态变量
来源：http://qyb.chenlongwang.top


<!-- 参考信息 -->