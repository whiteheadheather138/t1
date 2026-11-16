代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ztl.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://dew.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mfc.zdbjq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ynk.guowangkeji.top

[Q61] 移动平均
来源：http://kif.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gmr.xuanzx.com

[Q62] 分组占比
来源：http://mzj.feifeiyinyue.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xym.hammf.cn

[Q63] 开启事务
来源：http://wrp.sufxvd.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oip.aizwys.cn

[Q64] 提交事务
来源：http://gza.jinghuilouyu.cn

COMMIT;
来源：http://vmm.jqgufenzy.top

[Q65] 回滚事务
来源：http://kew.kuanghao11.cn

ROLLBACK;
来源：http://gir.ivvv.top

[Q66] 行锁查询
来源：http://ziq.sxryk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lmg.yj20258.top

[Q67] 设置隔离级别
来源：http://fcx.316326.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://her.chenlongwang.top

[Q68] 保存点
来源：http://djl.jinqigufen.top

SAVEPOINT sp1;
来源：http://jjn.tian-w.cn

ROLLBACK TO sp1;
来源：http://sll.pengpengdd.cyou

[Q69] 查看执行计划
来源：http://iwl.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xdt.cucudq.cn

[Q70] 更新统计信息
来源：http://gki.mhx1999.top

ANALYZE TABLE users;
来源：http://lhw.fanxiaobao.xyz

[Q71] 查看建表语句
来源：http://lyi.ydzc1.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gun.cheryme.top

[Q72] 查看索引
来源：http://fof.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://eko.ydjk.org.cn

[Q73] 查看表状态
来源：http://pph.chenzaomai.com

SHOW TABLE STATUS LIKE 'users';
来源：http://mhb.tarul.cn

[Q74] 强制使用索引
来源：http://jhe.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ojg.c1oappe.top

[Q75] 日期格式化
来源：http://hes.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://suu.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mpt.c1oappe.top

[Q76] 按天统计
来源：http://lye.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hmt.feifeiyinyue.top

[Q77] 时间加减
来源：http://pkd.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fvz.52xcode.cn

[Q78] 当前时间
来源：http://zcq.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lop.sjlbkw.cn

[Q79] 字符串拼接
来源：http://ofy.nwbrower.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zka.jianghu66.top

[Q80] 字符串截取
来源：http://xdb.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://prc.ehwqpu.com

[Q81] 字符串替换
来源：http://htw.cucudq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lhn.pycfn.com

[Q82] 字符长度与字节长度
来源：http://tnm.zhengqikj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hbo.zhijiandao.cn

[Q83] 大小写转换
来源：http://xvm.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tkt.havefunace.top

[Q84] 去除首尾空格
来源：http://htk.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://yhh.fanxiaobao.xyz

[Q85] 数值取整
来源：http://eqt.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wor.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://sxs.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gbw.zycfv.cn

[Q87] JSON 字段做条件
来源：http://pzb.chenzaomai.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jgf.zhengqikj.top

[Q88] 行转列（条件聚合）
来源：http://auw.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lcl.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://spr.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://bvc.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://juk.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://yec.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oaf.jyoumei.cn

================================================================================
来源：http://wlf.birdmap.top

R. Bash 专题
来源：http://hzs.c1oappe.top

================================================================================
来源：http://wra.feifeiyinyue.top

[R01] shebang 与严格模式
来源：http://rle.hammf.cn

#!/usr/bin/env bash
来源：http://wfr.yj20258.top

set -euo pipefail
来源：http://heh.fehbvm.com

[R02] 变量赋值与使用
来源：http://tvj.zhengqikj.top

name="Tom"; echo "$name"
来源：http://xfd.nanxinkj.top

[R03] 只读变量
来源：http://bum.guannengcc.top

readonly PI=3.14
来源：http://sbz.sysykeji.top

[R04] 位置参数
来源：http://qrx.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://spm.yongpay.top

[R05] 参数默认值
来源：http://vmr.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://tga.quarkkingdee.top

[R06] 判断命令是否存在
来源：http://jbe.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qnv.aibaodan.cn

[R07] if 判断文件
来源：http://zgi.daxiang520.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://paw.wangshuangyany.cn

[R08] 数值比较
来源：http://fyb.zdbjq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://esu.uphjek.com

[R09] 字符串比较
来源：http://dny.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xno.meibo888.top

[R10] 正则匹配
来源：http://agd.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://haf.zdbjq.cn

[R11] case 多分支
来源：http://dyl.hfpthk.cn

case "$1" in
来源：http://pxo.yj20258.top

start) echo "启动" ;;
来源：http://vti.cashguo.top

stop)  echo "停止" ;;
来源：http://jaj.meibo888.top

*)     echo "未知命令" ;;
来源：http://dvf.jyoumei.cn

esac
来源：http://bnk.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://oyo.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://brm.cashguo.top

[R13] for 计数循环
来源：http://tql.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://egk.yanxiufei.cn

[R14] C 风格 for
来源：http://nmg.sysykeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bng.zycfv.cn

[R15] while 逐行读文件
来源：http://nnh.yfazqb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://unr.xziqi.cn

[R16] until 等待条件
来源：http://tvj.hnqzz.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zna.yfazqb.com

[R17] 数组定义与取值
来源：http://khi.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://gjg.aibaodan.cn

[R18] 遍历数组
来源：http://rah.chenlongwang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fhv.epnwcf.com

[R19] 数组长度
来源：http://das.meibo888.top

echo "${#arr[@]}"
来源：http://hal.shuidangran.top

[R20] 关联数组（字典）
来源：http://vkr.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pcn.yuanzhike.top

[R21] 字符串长度
来源：http://qfx.cheryme.top

echo "${#s}"
来源：http://xaz.haohaochexian.top

[R22] 截取子串
来源：http://lex.aizwys.cn

echo "${s:0:5}"
来源：http://xgz.meibo888.top

[R23] 字符串替换
来源：http://kxk.cashguo.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ypf.gogol.net.cn

[R24] 大小写转换
来源：http://bif.jinyuanbaomall.cn

echo "${s^^}"; echo "${s,,}"
来源：http://soq.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://cue.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://awb.cdnleiting.top

[R26] 命令替换
来源：http://ddj.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://bhh.vqdsnc.cn

[R27] 算术展开
来源：http://pij.yuanzhike.top

echo $((1 + 2 * 3))
来源：http://uqu.jianghu66.top

[R28] 浮点运算
来源：http://kpt.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://gkp.zhixingplan.top

[R29] 定义函数
来源：http://lht.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yse.quarkkingdee.top

[R30] 函数返回状态码
来源：http://ufy.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://azj.hysaishi.cn

[R31] 局部变量
来源：http://ioo.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://lqp.jianghu66.top

[R32] 参数个数校验
来源：http://srf.vehdjk.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yuj.nanxuanxn.top

[R33] 捕获错误并提示行号
来源：http://orz.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zau.zhengqikj.top

[R34] 退出时清理
来源：http://nwf.nanxuanxn.top

trap 'rm -f "$tmp"' EXIT
来源：http://ltc.vehdjk.com

[R35] 后台执行并等待
来源：http://jxf.iojbl.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pla.fktsv.cn

[R36] 并发执行多个任务
来源：http://vqx.zdqjudy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bla.iojbl.cn

[R37] 把输出赋给变量
来源：http://bln.yj202588.top

files=$(ls -1)
来源：http://kum.vqdsnc.cn

[R38] 管道串联
来源：http://iyf.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://nic.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://asw.xylfe.cn

cmd > out.log 2>&1
来源：http://jeg.yuanzhike.top

[R40] 追加写日志
来源：http://pyx.jinqigfzy.top

echo "log" >> out.log
来源：http://cgd.nwbrower.top

[R41] 丢弃输出
来源：http://aiz.gzhubu.top

cmd >/dev/null 2>&1
来源：http://dzo.hfpthk.cn

[R42] 输入重定向
来源：http://lid.chenzaomai.com

wc -l < a.txt
来源：http://uoz.fktsv.cn

[R43] 按名字查找文件
来源：http://oap.uphjek.com

find . -name "*.log" -type f
来源：http://yyk.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://wlh.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://kni.ywan-chungtsiang.top

[R45] 批量删除
来源：http://imn.zhixingplan.top

find . -name "*.tmp" -delete
来源：http://npo.fanxiaobao.xyz

[R46] 递归替换文件内容
来源：http://rsj.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yyg.yongpay.top

[R47] sed 单行替换
来源：http://xne.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://zrj.xuetiantiany.cn

[R48] awk 取指定列
来源：http://gzq.birdmap.top

awk '{print $1, $3}' a.txt
来源：http://uzr.daria6918.cn

[R49] awk 带条件
来源：http://brr.daxiang520.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hrb.vehdjk.com

[R50] awk 求和
来源：http://lbd.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xgn.haohaochexian.top

[R51] 排序去重取前几
来源：http://qqu.hfpthk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jly.gaohongyu789.top

[R52] 统计行数
来源：http://vcq.yanxiufei.cn

wc -l a.txt
来源：http://svf.tian-w.cn

[R53] 查看文件头与实时尾
来源：http://ack.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uth.zhiwuduotai.top

[R54] 比较两个文件
来源：http://zhv.0kj1m.cn

diff a.txt b.txt
来源：http://cfl.yonumen.top

[R55] 压缩与解压
来源：http://dvi.tian-w.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sgv.tanke756.top

[R56] 远程拷贝
来源：http://mga.zhijiandao.cn

scp file user@host:/path/
来源：http://vdu.aibaodan.cn

[R57] 远程执行命令
来源：http://wgj.sxryk.cn

ssh user@host 'uptime'
来源：http://ekr.yj20258.top

[R58] 下载文件
来源：http://jum.shanyushiyangtech.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://exj.yuxming.cn

[R59] 发 POST JSON
来源：http://qgv.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://msh.nwbrower.top

[R60] 只看 HTTP 状态码
来源：http://klc.yj202588.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rpf.sxryk.cn

[R61] 磁盘占用
来源：http://byo.birdmap.top

df -h;  du -sh *
来源：http://sxs.jinqigfzy.top

[R62] 找最占空间的文件
来源：http://ohu.jinyuanbaomall.cn

du -ah . | sort -rh | head -10
来源：http://wcg.yj20258.top

[R63] 内存与进程
来源：http://cho.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://wzn.ppjwa.cn

[R64] 结束进程
来源：http://orm.yueranfly.top

kill -9 $(pgrep -f app.py)
来源：http://zvi.iojbl.cn

[R65] 查看端口占用
来源：http://egq.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yjo.guannengcc.top

[R66] 定时任务
来源：http://ipo.yongpay.top

crontab -e;  crontab -l
来源：http://dgp.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://aql.yj20258.top

openssl rand -hex 16
来源：http://vdc.zdqjudy.top

[R68] 计算文件校验值
来源：http://pcr.sweek.top

sha256sum a.txt;  md5sum a.txt
来源：http://gnf.xuanzx.com

[R69] 生成随机密码
来源：http://eyc.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://evn.shzxlz.cn

[R70] 时间戳与互转
来源：http://saz.shuidangran.top

date +%s;  date -d @1700000000
来源：http://spr.sufxvd.cn

[R71] 日期格式化
来源：http://yul.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sbz.xuanzx.com

[R72] 等待端口就绪
来源：http://edv.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fso.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://htp.nanxinkj.top

split -l 1000 big.log part_
来源：http://wvn.feifeiyinyue.top

[R74] 批量重命名
来源：http://efh.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cvi.redwolf501.top

[R75] 导出环境变量
来源：http://xgx.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://sxu.fehbvm.com

[R76] 使用临时文件
来源：http://phu.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iwu.yongpay.top

[R77] 读取用户输入
来源：http://kne.316326.xyz

read -rp "请输入: " ans
来源：http://ncm.c1oappe.top

[R78] 交互式菜单
来源：http://cmd.cucudq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://azz.yonumen.top

[R79] 解析命令行选项
来源：http://htu.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pbc.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://rgc.fengsongda.top

time ./run.sh
来源：http://cvf.yanxiufei.cn

================================================================================
来源：http://dsh.ivvv.top

S. C / C++ 专题
来源：http://wba.pengpengdd.cyou

================================================================================
来源：http://qxb.316326.xyz

[S01] C：Hello World
来源：http://pry.zhoulong.xyz

#include <stdio.h>
来源：http://rke.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xms.zdbjq.cn

[S02] C：变量与格式化输出
来源：http://qln.haohaochexian.top

int a = 10; printf("%d\n", a);
来源：http://ayg.cqqwz.cn

[S03] C：读入整数
来源：http://mok.zhengqikj.top

int x; scanf("%d", &x);
来源：http://yxn.fengsongda.top

[S04] C：字符串复制
来源：http://zjb.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bjv.zhengqikj.top

[S05] C：字符串长度
来源：http://pwe.sysykeji.top

strlen(s)
来源：http://mwy.daxiang520.top

[S06] C：字符串比较
来源：http://bne.c1oappe.top

strcmp(a, b) == 0
来源：http://zwm.ctjpmb.com

[S07] C：数组遍历求和
来源：http://jog.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lsg.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://lne.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vye.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://kyx.snrcjt.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://suv.hesvh.cn

[S10] C：指针与解引用
来源：http://dzn.c1oappe.top

int *p = &a;  *p = 5;
来源：http://tbj.chenlongwang.top

[S11] C：逐行读文件
来源：http://efp.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://mcj.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lty.ctjpmb.com

fclose(f);
来源：http://nyl.hfpthk.cn

[S12] C：写文件
来源：http://fib.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sqq.vqdsnc.cn

[S13] C：宏定义
来源：http://ook.ctjpmb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tcx.yuxming.cn

[S14] C：枚举
来源：http://qib.aizwys.cn

enum Color { RED, GREEN, BLUE };
来源：http://xcr.shanyushiyangtech.top

[S15] C：类型转换
来源：http://ohb.hammf.cn

(double) a / b
来源：http://ksh.xinyue.icu

[S16] C：位操作置位
来源：http://dck.yongpay.top

x |= (1 << 3);
来源：http://kpb.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://log.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wdk.wangshuangyany.cn

[S18] C：命令行参数
来源：http://hph.sjlbkw.cn

int main(int argc, char **argv)
来源：http://dlb.yonumen.top

[S19] C：快速排序
来源：http://brs.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dnp.9152youxi.cn

[S20] C：二分查找
来源：http://nut.shuidangran.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://prt.gotoacloud.top

[S21] C：字符类别判断
来源：http://ptu.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hdm.wangdashe.top

[S22] C：字符串转数字
来源：http://gsu.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://eiz.xuanzx.com

[S23] C：随机数
来源：http://khp.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mok.52xcode.cn

[S24] C：获取本地时间
来源：http://kwu.cucudq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gbs.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://abf.yvedp.cn

memcpy(dst, src, n);
来源：http://ayz.hysaishi.cn

[S26] C：内存清零
来源：http://ezc.jyoumei.cn

memset(a, 0, sizeof a);
来源：http://wws.xuetiantiany.cn

[S27] C：定义常量
来源：http://uxq.xuetiantiany.cn

const double PI = 3.14159;
来源：http://nlz.cheryme.top

[S28] C：静态变量
来源：http://kvw.xinyue.icu

static int counter = 0;
来源：http://mud.yj20258888.top

[S29] C：变参函数
来源：http://wky.uphjek.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rdi.shuidangran.top

[S30] C：头文件保护
来源：http://pwq.yuanzhike.top


<!-- 参考信息 -->