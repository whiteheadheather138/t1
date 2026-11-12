代发 wailian999

[Q63] 开启事务
来源：http://ekt.guannengcc.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rgt.mhx1999.top

[Q64] 提交事务
来源：http://iln.shuidangran.top

COMMIT;
来源：http://ssm.xuetiantiany.cn

[Q65] 回滚事务
来源：http://egd.bjfxy.top

ROLLBACK;
来源：http://arp.yfazqb.com

[Q66] 行锁查询
来源：http://aec.sufxvd.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xhd.zhengqikj.top

[Q67] 设置隔离级别
来源：http://bur.haohaochexian.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ioh.dashuyun.cn

[Q68] 保存点
来源：http://jyr.yj20258888.top

SAVEPOINT sp1;
来源：http://sta.tarul.cn

ROLLBACK TO sp1;
来源：http://mim.fengsongda.top

[Q69] 查看执行计划
来源：http://sxs.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ele.fktsv.cn

[Q70] 更新统计信息
来源：http://jvb.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://jwz.ivvv.top

[Q71] 查看建表语句
来源：http://epe.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pfr.vehdjk.com

[Q72] 查看索引
来源：http://uzp.zhoulong.xyz

SHOW INDEX FROM users;
来源：http://wgf.zdqjudy.top

[Q73] 查看表状态
来源：http://boz.guannengcc.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fwn.sxryk.cn

[Q74] 强制使用索引
来源：http://mjx.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jpo.shanyushiyangtech.top

[Q75] 日期格式化
来源：http://gbn.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gho.yanxiufei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nnz.gzhubu.top

[Q76] 按天统计
来源：http://kxg.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ryx.sysykeji.top

[Q77] 时间加减
来源：http://qsr.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tie.cdnleiting.top

[Q78] 当前时间
来源：http://rzp.ydzc1.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hof.ehwqpu.com

[Q79] 字符串拼接
来源：http://bmb.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bix.hongshengwenyu.top

[Q80] 字符串截取
来源：http://dnp.sufxvd.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ufz.c1oappe.top

[Q81] 字符串替换
来源：http://imx.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ypp.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://fct.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pjq.pengpengdd.cyou

[Q83] 大小写转换
来源：http://jvj.iojbl.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tiq.hnxiangtu.top

[Q84] 去除首尾空格
来源：http://fst.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://cez.fktsv.cn

[Q85] 数值取整
来源：http://xeb.yangfankeji.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hhb.tianlin.xyz

[Q86] 读取 JSON 字段
来源：http://evj.ppjwa.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wdt.mhx1999.top

[Q87] JSON 字段做条件
来源：http://hib.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tzm.xuanzx.com

[Q88] 行转列（条件聚合）
来源：http://uwc.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://urf.iojbl.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sxd.ybcxt.top

[Q89] 判断表是否存在
来源：http://mkf.wangdashe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ppp.ivvv.top

[Q90] 生成序号列
来源：http://fgz.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://amm.smart0.xyz

================================================================================
来源：http://dfn.shuidangran.top

R. Bash 专题
来源：http://pej.shzxlz.cn

================================================================================
来源：http://pna.ivvv.top

[R01] shebang 与严格模式
来源：http://twg.yonumen.top

#!/usr/bin/env bash
来源：http://wgw.snrcjt.cn

set -euo pipefail
来源：http://spw.yanxiufei.cn

[R02] 变量赋值与使用
来源：http://gct.ydzc1.top

name="Tom"; echo "$name"
来源：http://imq.fzhhl.top

[R03] 只读变量
来源：http://ces.9152youxi.cn

readonly PI=3.14
来源：http://fqv.shzxlz.cn

[R04] 位置参数
来源：http://dpq.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pky.jyoumei.cn

[R05] 参数默认值
来源：http://xgy.fzhhl.top

name="${1:-default}"
来源：http://cdy.hcnkem.com

[R06] 判断命令是否存在
来源：http://guk.iojbl.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nia.fehbvm.com

[R07] if 判断文件
来源：http://yld.guannengcc.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mcm.chenzaomai.com

[R08] 数值比较
来源：http://avu.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://skc.hnxiangtu.top

[R09] 字符串比较
来源：http://jhs.hnxiangtu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zbg.zhengqikj.top

[R10] 正则匹配
来源：http://ved.dianchejie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oaz.fzhhl.top

[R11] case 多分支
来源：http://cdm.hcnkem.com

case "$1" in
来源：http://gzz.yongpay.top

start) echo "启动" ;;
来源：http://nyj.xuetiantiany.cn

stop)  echo "停止" ;;
来源：http://lte.gzhubu.top

*)     echo "未知命令" ;;
来源：http://rjy.sjlbkw.cn

esac
来源：http://olu.hywenlv.cn

[R12] for 遍历文件
来源：http://siu.ivvv.top

for f in *.txt; do echo "$f"; done
来源：http://ecu.wangdashe.top

[R13] for 计数循环
来源：http://sxc.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://rxu.vqdsnc.cn

[R14] C 风格 for
来源：http://mfs.52xcode.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yfu.jianghu66.top

[R15] while 逐行读文件
来源：http://xdd.gogol.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ibx.shuidangran.top

[R16] until 等待条件
来源：http://csj.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wii.yonumen.top

[R17] 数组定义与取值
来源：http://hoy.yangfankeji.com

arr=(a b c); echo "${arr[0]}"
来源：http://zje.hnxiangtu.top

[R18] 遍历数组
来源：http://uwi.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wnq.quarkkingdee.top

[R19] 数组长度
来源：http://qaj.9152youxi.cn

echo "${#arr[@]}"
来源：http://lbv.hfpthk.cn

[R20] 关联数组（字典）
来源：http://pzb.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://azx.sysykeji.top

[R21] 字符串长度
来源：http://leu.chenjidiqi.icu

echo "${#s}"
来源：http://zlh.xingfuxueyuan.xyz

[R22] 截取子串
来源：http://ned.smart0.xyz

echo "${s:0:5}"
来源：http://ipk.ehwqpu.com

[R23] 字符串替换
来源：http://zow.sysykeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ypp.xuetiantiany.cn

[R24] 大小写转换
来源：http://igl.ydzc1.top

echo "${s^^}"; echo "${s,,}"
来源：http://uiz.hcnkem.com

[R25] 去后缀 / 去前缀
来源：http://fol.guannengcc.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://yqf.zhoulong.xyz

[R26] 命令替换
来源：http://zqp.jiagoushi.top

now=$(date +%F); echo "$now"
来源：http://cuw.iojbl.cn

[R27] 算术展开
来源：http://zyh.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://xzx.chenlongwang.top

[R28] 浮点运算
来源：http://skf.quarkkingdee.top

echo "scale=2; 10/3" | bc
来源：http://chv.havefunace.top

[R29] 定义函数
来源：http://wdd.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rsy.shangyingyoupin.top

[R30] 函数返回状态码
来源：http://kvp.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://pay.hfpthk.cn

[R31] 局部变量
来源：http://chp.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://hee.nanxinkj.top

[R32] 参数个数校验
来源：http://zoj.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://phs.havefunace.top

[R33] 捕获错误并提示行号
来源：http://zim.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bgt.pycfn.com

[R34] 退出时清理
来源：http://cjv.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nzh.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://qqt.hammf.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hsu.hesvh.cn

[R36] 并发执行多个任务
来源：http://sjk.jinghuilouyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yde.snrcjt.cn

[R37] 把输出赋给变量
来源：http://vxa.aibaodan.cn

files=$(ls -1)
来源：http://wqm.dianchejie.cn

[R38] 管道串联
来源：http://pdt.gzhubu.top

cat a.txt | grep -i error | wc -l
来源：http://dlw.guowangkeji.top

[R39] 重定向标准输出与错误
来源：http://hcn.yongpay.top

cmd > out.log 2>&1
来源：http://bqz.yuanzhike.top

[R40] 追加写日志
来源：http://bjk.hongshengwenyu.top

echo "log" >> out.log
来源：http://urx.yfazqb.com

[R41] 丢弃输出
来源：http://kdz.shangyingyoupin.top

cmd >/dev/null 2>&1
来源：http://qzk.pycfn.com

[R42] 输入重定向
来源：http://ujz.zhaomingkeji.xyz

wc -l < a.txt
来源：http://tgb.ehwqpu.com

[R43] 按名字查找文件
来源：http://wxs.jinqigufen.top

find . -name "*.log" -type f
来源：http://acz.316326.xyz

[R44] 按修改时间查找
来源：http://eaj.fktsv.cn

find . -mtime -7 -type f
来源：http://ptd.yj20258888.top

[R45] 批量删除
来源：http://uqk.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://dof.ppjwa.cn

[R46] 递归替换文件内容
来源：http://chv.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dmv.yangfankeji.com

[R47] sed 单行替换
来源：http://tie.guannengcc.top

sed -i 's/foo/bar/g' a.txt
来源：http://xjs.bjfxy.top

[R48] awk 取指定列
来源：http://ora.yongpay.top

awk '{print $1, $3}' a.txt
来源：http://wdt.sysykeji.top

[R49] awk 带条件
来源：http://rvd.yanxiufei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rnh.bbcook.cn

[R50] awk 求和
来源：http://ymq.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ysl.ydzc1.top

[R51] 排序去重取前几
来源：http://vzh.mhx1999.top

sort a.txt | uniq -c | sort -rn | head
来源：http://miq.ppjwa.cn

[R52] 统计行数
来源：http://rvt.guannengcc.top

wc -l a.txt
来源：http://viy.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://sde.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://obs.hcnkem.com

[R54] 比较两个文件
来源：http://rus.yj20258.top

diff a.txt b.txt
来源：http://jkn.gaohongyu789.top

[R55] 压缩与解压
来源：http://hwg.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ges.sysykeji.top

[R56] 远程拷贝
来源：http://tck.gaohongyu789.top

scp file user@host:/path/
来源：http://hwb.xuetiantiany.cn

[R57] 远程执行命令
来源：http://dbr.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://tpq.zdqjudy.top

[R58] 下载文件
来源：http://ozd.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qxy.havefunace.top

[R59] 发 POST JSON
来源：http://lgk.nanxuanxn.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qkd.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://qgd.52xcode.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wdn.cucudq.cn

[R61] 磁盘占用
来源：http://jmv.zdbjq.cn

df -h;  du -sh *
来源：http://lsg.yj20258888.top

[R62] 找最占空间的文件
来源：http://rmb.yj20258.top

du -ah . | sort -rh | head -10
来源：http://aom.zhoulong.xyz

[R63] 内存与进程
来源：http://ndy.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://sst.52xcode.cn

[R64] 结束进程
来源：http://yzk.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://tpl.snrcjt.cn

[R65] 查看端口占用
来源：http://qit.pengpengdd.cyou

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tdm.snrcjt.cn

[R66] 定时任务
来源：http://mww.mhx1999.top

crontab -e;  crontab -l
来源：http://owo.sweek.top

[R67] 生成随机十六进制串
来源：http://mfd.yuanzhike.top

openssl rand -hex 16
来源：http://bkb.ybcxt.top

[R68] 计算文件校验值
来源：http://fwc.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://djc.shanyushiyangtech.top

[R69] 生成随机密码
来源：http://vfj.guannengcc.top

head -c 16 /dev/urandom | base64
来源：http://eng.wangdashe.top

[R70] 时间戳与互转
来源：http://rja.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://bxq.yj202588.top

[R71] 日期格式化
来源：http://ecg.ivvv.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sar.aibaodan.cn

[R72] 等待端口就绪
来源：http://wyg.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yyh.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://wzi.yj202588.top

split -l 1000 big.log part_
来源：http://twn.cheryme.top

[R74] 批量重命名
来源：http://cog.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ccy.aibaodan.cn

[R75] 导出环境变量
来源：http://bdx.aizwys.cn

export PATH="$HOME/bin:$PATH"
来源：http://wfo.vehdjk.com

[R76] 使用临时文件
来源：http://ybs.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jhe.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://hkt.smart0.xyz

read -rp "请输入: " ans
来源：http://atw.gotoacloud.top

[R78] 交互式菜单
来源：http://iiw.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ehf.shzxlz.cn

[R79] 解析命令行选项
来源：http://pbz.chenlongwang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uyt.jqgfzy.top

[R80] 查看脚本执行耗时
来源：http://enp.ywan-chungtsiang.top

time ./run.sh
来源：http://rmm.cucudq.cn

================================================================================
来源：http://ikn.yj20258888.top

S. C / C++ 专题
来源：http://wbc.fengsongda.top

================================================================================
来源：http://mzp.guannengcc.top

[S01] C：Hello World
来源：http://liz.zhongyouzk.top

#include <stdio.h>
来源：http://sqq.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://snw.316326.xyz

[S02] C：变量与格式化输出
来源：http://afm.hesvh.cn

int a = 10; printf("%d\n", a);
来源：http://vdg.bbcook.cn

[S03] C：读入整数
来源：http://vrr.yueranfly.top

int x; scanf("%d", &x);
来源：http://imo.nanxuanxn.top

[S04] C：字符串复制
来源：http://taq.hesvh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jip.zdqjudy.top

[S05] C：字符串长度
来源：http://yfd.chenzaomai.com

strlen(s)
来源：http://vkf.hnqzz.top

[S06] C：字符串比较
来源：http://poe.shzxlz.cn

strcmp(a, b) == 0
来源：http://dmp.yuxming.cn

[S07] C：数组遍历求和
来源：http://gpu.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bwl.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://qwy.0kj1m.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uwe.tarul.cn

[S09] C：结构体定义与初始化
来源：http://pwu.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yfl.sufxvd.cn

[S10] C：指针与解引用
来源：http://dth.zhengqikj.top

int *p = &a;  *p = 5;
来源：http://uxx.ctjpmb.com

[S11] C：逐行读文件
来源：http://xgk.pengpengdd.cyou

FILE *f = fopen("a.txt", "r");
来源：http://ntv.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qxo.hysaishi.cn

fclose(f);
来源：http://sko.fengsongda.top

[S12] C：写文件
来源：http://bho.yonumen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://skt.zdqjudy.top

[S13] C：宏定义
来源：http://eaa.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rwp.jinyuanbaomall.cn

[S14] C：枚举
来源：http://gow.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://fkq.kuanghao11.cn

[S15] C：类型转换
来源：http://eei.nwbrower.top

(double) a / b
来源：http://rwv.birdmap.top

[S16] C：位操作置位
来源：http://tak.fanxiaobao.xyz

x |= (1 << 3);
来源：http://phv.cdnleiting.top

[S17] C：安全拼接字符串
来源：http://bpe.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gmw.316326.xyz

[S18] C：命令行参数
来源：http://ucl.jqgufenzy.top

int main(int argc, char **argv)
来源：http://ouk.hesvh.cn

[S19] C：快速排序
来源：http://kxg.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://syy.yvedp.cn

[S20] C：二分查找
来源：http://rar.uphjek.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bag.316326.xyz

[S21] C：字符类别判断
来源：http://jlo.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jei.jianghu66.top

[S22] C：字符串转数字
来源：http://gzd.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eoi.aizwys.cn

[S23] C：随机数
来源：http://zew.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fuc.haohaochexian.top

[S24] C：获取本地时间
来源：http://kye.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xwo.nanxinkj.top

[S25] C：内存拷贝
来源：http://mki.hesvh.cn

memcpy(dst, src, n);
来源：http://zhg.chenjidiqi.icu

[S26] C：内存清零
来源：http://qba.jyoumei.cn

memset(a, 0, sizeof a);
来源：http://xhd.zdqjudy.top

[S27] C：定义常量
来源：http://jsu.tarul.cn

const double PI = 3.14159;
来源：http://tdm.havefunace.top

[S28] C：静态变量
来源：http://cae.xylfe.cn

static int counter = 0;
来源：http://jzz.wangshuangyany.cn

[S29] C：变参函数
来源：http://xsm.hnqzz.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wjp.tarul.cn

[S30] C：头文件保护
来源：http://smt.hammf.cn

#ifndef X_H
来源：http://fpl.chenlongwang.top

#define X_H
来源：http://kqa.redwolf501.top

#endif
来源：http://vii.hesvh.cn

[S31] C++：Hello World
来源：http://vby.vqdsnc.cn

#include <iostream>
来源：http://neh.fanxiaobao.xyz

int main() { std::cout << "Hello\n"; }
来源：http://ztz.shanyushiyangkeji.top

[S32] C++：字符串
来源：http://kpe.hammf.cn

std::string s = "hi";  s += "!";
来源：http://dla.jinghuilouyu.cn


<!-- 参考信息 -->