代发 wailian999

[Q63] 开启事务
来源：http://jms.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wzd.hammf.cn

[Q64] 提交事务
来源：http://dpi.daxiang520.top

COMMIT;
来源：http://ndq.aizwys.cn

[Q65] 回滚事务
来源：http://mlh.ybcxt.top

ROLLBACK;
来源：http://eyk.chenzaomai.com

[Q66] 行锁查询
来源：http://szr.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jpx.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://vmy.jyoumei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bav.52xcode.cn

[Q68] 保存点
来源：http://pfq.nanxuanxn.top

SAVEPOINT sp1;
来源：http://uuu.daria6918.cn

ROLLBACK TO sp1;
来源：http://elm.yfazqb.com

[Q69] 查看执行计划
来源：http://gae.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yao.kuanghao11.cn

[Q70] 更新统计信息
来源：http://aav.xziqi.cn

ANALYZE TABLE users;
来源：http://nrt.shuidangran.top

[Q71] 查看建表语句
来源：http://dwl.fzhhl.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uyx.chenzaomai.com

[Q72] 查看索引
来源：http://tst.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://ckq.ppjwa.cn

[Q73] 查看表状态
来源：http://jpq.jlsjyb.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uhk.jinghuilouyu.cn

[Q74] 强制使用索引
来源：http://rzz.feifeiyinyue.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cxa.bbcook.cn

[Q75] 日期格式化
来源：http://nvw.birdmap.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wai.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vex.yuxming.cn

[Q76] 按天统计
来源：http://wuy.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ijc.shanyushiyangkeji.top

[Q77] 时间加减
来源：http://cyt.jinqigfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hac.uphjek.com

[Q78] 当前时间
来源：http://hrv.andypj.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tdr.yuxming.cn

[Q79] 字符串拼接
来源：http://kkc.fzhhl.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ryz.hnqzz.top

[Q80] 字符串截取
来源：http://mqv.nwbrower.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zac.yfazqb.com

[Q81] 字符串替换
来源：http://yoz.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uba.tarul.cn

[Q82] 字符长度与字节长度
来源：http://ern.hammf.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bzj.yuxming.cn

[Q83] 大小写转换
来源：http://guq.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zhz.bbcook.cn

[Q84] 去除首尾空格
来源：http://vsz.zhengqikj.top

SELECT TRIM(name) FROM users;
来源：http://pxz.jinqigufen.top

[Q85] 数值取整
来源：http://wua.ivvv.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uel.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://egj.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nso.shzxlz.cn

[Q87] JSON 字段做条件
来源：http://rrq.jinqigfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oxt.hesvh.cn

[Q88] 行转列（条件聚合）
来源：http://pci.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rzn.hysaishi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yvn.52xcode.cn

[Q89] 判断表是否存在
来源：http://ylt.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bap.yj20258.top

[Q90] 生成序号列
来源：http://deo.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hus.shanyushiyangkeji.top

================================================================================
来源：http://xpx.fktsv.cn

R. Bash 专题
来源：http://vuy.quarkkingdee.top

================================================================================
来源：http://iqg.52xcode.cn

[R01] shebang 与严格模式
来源：http://cga.jinqigufen.top

#!/usr/bin/env bash
来源：http://tpk.hnxiangtu.top

set -euo pipefail
来源：http://hif.xylfe.cn

[R02] 变量赋值与使用
来源：http://qbr.yj20258.top

name="Tom"; echo "$name"
来源：http://lop.fktsv.cn

[R03] 只读变量
来源：http://kph.smart0.xyz

readonly PI=3.14
来源：http://ufj.ywan-chungtsiang.top

[R04] 位置参数
来源：http://gah.andypj.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dvi.hfpthk.cn

[R05] 参数默认值
来源：http://dyr.yangfankeji.com

name="${1:-default}"
来源：http://wle.cucudq.cn

[R06] 判断命令是否存在
来源：http://sxt.jqgfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xte.epnwcf.com

[R07] if 判断文件
来源：http://nsv.zhoulong.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yfr.svipenyu.cn

[R08] 数值比较
来源：http://akc.0kj1m.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gsx.fzhhl.top

[R09] 字符串比较
来源：http://yqt.uphjek.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://say.hcnkem.com

[R10] 正则匹配
来源：http://thg.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://paj.redwolf501.top

[R11] case 多分支
来源：http://ued.52xcode.cn

case "$1" in
来源：http://qen.hnqzz.top

start) echo "启动" ;;
来源：http://moa.zhiwuduotai.top

stop)  echo "停止" ;;
来源：http://edn.hfpthk.cn

*)     echo "未知命令" ;;
来源：http://nyb.kuanghao11.cn

esac
来源：http://wio.xylfe.cn

[R12] for 遍历文件
来源：http://qsj.chenzaomai.com

for f in *.txt; do echo "$f"; done
来源：http://iaq.yj20258.top

[R13] for 计数循环
来源：http://gbn.ydjk.org.cn

for i in {1..10}; do echo "$i"; done
来源：http://nxl.9152youxi.cn

[R14] C 风格 for
来源：http://and.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pmv.cdnleiting.top

[R15] while 逐行读文件
来源：http://sbj.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pqm.shzxlz.cn

[R16] until 等待条件
来源：http://hdo.tian-w.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rnt.bjfxy.top

[R17] 数组定义与取值
来源：http://cqo.ppjwa.cn

arr=(a b c); echo "${arr[0]}"
来源：http://spr.tianlin.xyz

[R18] 遍历数组
来源：http://cjh.svipenyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jxf.shzxlz.cn

[R19] 数组长度
来源：http://ger.uphjek.com

echo "${#arr[@]}"
来源：http://qds.xylfe.cn

[R20] 关联数组（字典）
来源：http://bib.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://onp.redwolf501.top

[R21] 字符串长度
来源：http://wem.0kj1m.cn

echo "${#s}"
来源：http://tzu.jqgfzy.top

[R22] 截取子串
来源：http://ajl.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://pcs.hnxiangtu.top

[R23] 字符串替换
来源：http://zbf.zhiwuduotai.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://soo.vqdsnc.cn

[R24] 大小写转换
来源：http://jte.haohaochexian.top

echo "${s^^}"; echo "${s,,}"
来源：http://akd.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://igy.mhx1999.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qou.shanyushiyangtech.top

[R26] 命令替换
来源：http://trv.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://jmu.yfazqb.com

[R27] 算术展开
来源：http://lbx.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://clx.iojbl.cn

[R28] 浮点运算
来源：http://xhx.yj20258.top

echo "scale=2; 10/3" | bc
来源：http://atv.jinqigufen.top

[R29] 定义函数
来源：http://vtc.zhoulong.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://izv.zhijiandao.cn

[R30] 函数返回状态码
来源：http://mts.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://jxc.cucudq.cn

[R31] 局部变量
来源：http://nen.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://tmz.zhoulong.xyz

[R32] 参数个数校验
来源：http://avv.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://niw.tarul.cn

[R33] 捕获错误并提示行号
来源：http://dcx.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gkn.quarkkingdee.top

[R34] 退出时清理
来源：http://vou.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://tgc.xinyue.icu

[R35] 后台执行并等待
来源：http://xed.pengpengdd.cyou

sleep 5 & pid=$!; wait "$pid"
来源：http://szn.ctjpmb.com

[R36] 并发执行多个任务
来源：http://ssz.andypj.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wce.xziqi.cn

[R37] 把输出赋给变量
来源：http://kwl.shuidangran.top

files=$(ls -1)
来源：http://taz.yj20258888.top

[R38] 管道串联
来源：http://hdw.hywenlv.cn

cat a.txt | grep -i error | wc -l
来源：http://ymw.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://pwn.jinqigfzy.top

cmd > out.log 2>&1
来源：http://imc.yueranfly.top

[R40] 追加写日志
来源：http://rpn.c1oappe.top

echo "log" >> out.log
来源：http://bvs.meibo888.top

[R41] 丢弃输出
来源：http://ozq.nwbrower.top

cmd >/dev/null 2>&1
来源：http://trx.hammf.cn

[R42] 输入重定向
来源：http://mna.nanxinkj.top

wc -l < a.txt
来源：http://fcs.zhongyouzk.top

[R43] 按名字查找文件
来源：http://bws.fengsongda.top

find . -name "*.log" -type f
来源：http://nst.quarkkingdee.top

[R44] 按修改时间查找
来源：http://mkl.tianlin.xyz

find . -mtime -7 -type f
来源：http://bex.guannengcc.top

[R45] 批量删除
来源：http://xdu.zhaomingkeji.xyz

find . -name "*.tmp" -delete
来源：http://erx.andypj.xyz

[R46] 递归替换文件内容
来源：http://zsa.hongshengwenyu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://smf.mhx1999.top

[R47] sed 单行替换
来源：http://vbl.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://zdm.gzhubu.top

[R48] awk 取指定列
来源：http://uxs.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://qxt.gzhubu.top

[R49] awk 带条件
来源：http://wrt.ehwqpu.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fqj.yj20258888.top

[R50] awk 求和
来源：http://usn.kuanghao11.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kdb.shzxlz.cn

[R51] 排序去重取前几
来源：http://dad.ppjwa.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dwm.epnwcf.com

[R52] 统计行数
来源：http://kls.hysaishi.cn

wc -l a.txt
来源：http://sci.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://vtc.haohaochexian.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sbv.gzhubu.top

[R54] 比较两个文件
来源：http://ekh.hfpthk.cn

diff a.txt b.txt
来源：http://uaz.tarul.cn

[R55] 压缩与解压
来源：http://qrj.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ofh.sxryk.cn

[R56] 远程拷贝
来源：http://lyw.jinghuilouyu.cn

scp file user@host:/path/
来源：http://jko.jqgfzy.top

[R57] 远程执行命令
来源：http://wum.yuanzhike.top

ssh user@host 'uptime'
来源：http://vzb.sufxvd.cn

[R58] 下载文件
来源：http://nkc.jyoumei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://noa.meibo888.top

[R59] 发 POST JSON
来源：http://zrf.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jde.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://jrg.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uio.hnqzz.top

[R61] 磁盘占用
来源：http://zvb.yanxiufei.cn

df -h;  du -sh *
来源：http://duc.yj20258.top

[R62] 找最占空间的文件
来源：http://rze.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://bxk.jqgufenzy.top

[R63] 内存与进程
来源：http://ere.sufxvd.cn

free -h;  ps aux | grep nginx
来源：http://zhq.snrcjt.cn

[R64] 结束进程
来源：http://dju.zdqjudy.top

kill -9 $(pgrep -f app.py)
来源：http://xit.yonumen.top

[R65] 查看端口占用
来源：http://hgy.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kda.zhongyouzk.top

[R66] 定时任务
来源：http://wnw.zdbjq.cn

crontab -e;  crontab -l
来源：http://ayh.kuanghao11.cn

[R67] 生成随机十六进制串
来源：http://iod.jinqigufen.top

openssl rand -hex 16
来源：http://rxa.fzhhl.top

[R68] 计算文件校验值
来源：http://sub.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://cnl.wangshuangyany.cn

[R69] 生成随机密码
来源：http://yrg.ctjpmb.com

head -c 16 /dev/urandom | base64
来源：http://kdn.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://hhd.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://cdh.jinqigufen.top

[R71] 日期格式化
来源：http://uxp.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://stu.haohaochexian.top

[R72] 等待端口就绪
来源：http://qey.jinqigfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yhp.feifeiyinyue.top

[R73] 分割大日志
来源：http://oor.iojbl.cn

split -l 1000 big.log part_
来源：http://ufv.kuanghao11.cn

[R74] 批量重命名
来源：http://tzz.316326.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://imv.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://bvy.bjfxy.top

export PATH="$HOME/bin:$PATH"
来源：http://uwg.sjlbkw.cn

[R76] 使用临时文件
来源：http://kkz.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ifo.chenzaomai.com

[R77] 读取用户输入
来源：http://gyp.ywan-chungtsiang.top

read -rp "请输入: " ans
来源：http://vhm.0kj1m.cn

[R78] 交互式菜单
来源：http://anl.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gml.xylfe.cn

[R79] 解析命令行选项
来源：http://vac.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qty.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://zia.shzxlz.cn

time ./run.sh
来源：http://htx.hammf.cn

================================================================================
来源：http://dmo.jqgfzy.top

S. C / C++ 专题
来源：http://xsg.meibo888.top

================================================================================
来源：http://ubb.kuanghao11.cn

[S01] C：Hello World
来源：http://xji.fengsongda.top

#include <stdio.h>
来源：http://dbk.sweek.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tfv.hysaishi.cn

[S02] C：变量与格式化输出
来源：http://fmv.svipenyu.cn

int a = 10; printf("%d\n", a);
来源：http://ecf.cqqwz.cn

[S03] C：读入整数
来源：http://hov.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://emp.yj20258888.top

[S04] C：字符串复制
来源：http://hsw.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://vio.svipenyu.cn

[S05] C：字符串长度
来源：http://ejv.zhixingplan.top

strlen(s)
来源：http://hez.epnwcf.com

[S06] C：字符串比较
来源：http://gnq.jqgfzy.top

strcmp(a, b) == 0
来源：http://kai.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://bgn.fanxiaobao.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qei.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://mjl.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://irr.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://qoy.haohaochexian.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xzy.316326.xyz

[S10] C：指针与解引用
来源：http://bew.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://phu.zdbjq.cn

[S11] C：逐行读文件
来源：http://mro.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://bik.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ory.gogol.net.cn

fclose(f);
来源：http://uga.cqqwz.cn

[S12] C：写文件
来源：http://ncb.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xfg.ivvv.top

[S13] C：宏定义
来源：http://bas.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ewx.redwolf501.top

[S14] C：枚举
来源：http://bxm.yvedp.cn

enum Color { RED, GREEN, BLUE };
来源：http://uoh.epnwcf.com

[S15] C：类型转换
来源：http://vof.daxiang520.top

(double) a / b
来源：http://cmf.nanxuanxn.top

[S16] C：位操作置位
来源：http://aot.gzhubu.top

x |= (1 << 3);
来源：http://xln.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://flu.jinqigfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eor.jyoumei.cn

[S18] C：命令行参数
来源：http://nvf.hywenlv.cn

int main(int argc, char **argv)
来源：http://nph.52xcode.cn

[S19] C：快速排序
来源：http://eaw.yfazqb.com

qsort(a, n, sizeof(int), cmp);
来源：http://qmz.ehwqpu.com

[S20] C：二分查找
来源：http://eny.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bfr.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://zjn.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pna.c1oappe.top

[S22] C：字符串转数字
来源：http://hnh.dashuyun.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ygb.aizwys.cn

[S23] C：随机数
来源：http://pcb.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zhu.c1oappe.top

[S24] C：获取本地时间
来源：http://fht.sweek.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ejs.havefunace.top

[S25] C：内存拷贝
来源：http://uud.yuxming.cn

memcpy(dst, src, n);
来源：http://lro.nwbrower.top

[S26] C：内存清零
来源：http://srw.zycfv.cn

memset(a, 0, sizeof a);
来源：http://pbo.redwolf501.top

[S27] C：定义常量
来源：http://cxn.ivvv.top

const double PI = 3.14159;
来源：http://ewi.pycfn.com

[S28] C：静态变量
来源：http://poe.gogol.net.cn

static int counter = 0;
来源：http://vuv.kuanghao11.cn

[S29] C：变参函数
来源：http://mfe.fzhhl.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kkb.jinyuanbaomall.cn

[S30] C：头文件保护
来源：http://snw.jqgfzy.top

#ifndef X_H
来源：http://tkz.yfazqb.com

#define X_H
来源：http://ftl.aizwys.cn

#endif
来源：http://rga.feifeiyinyue.top

[S31] C++：Hello World
来源：http://eeq.c1oappe.top

#include <iostream>
来源：http://jch.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://syo.0kj1m.cn

[S32] C++：字符串
来源：http://ibk.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://ism.tianlin.xyz


<!-- 参考信息 -->