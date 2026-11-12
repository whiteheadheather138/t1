代发 wailian999

[Q65] 回滚事务
来源：http://yfs.fanxiaobao.xyz

ROLLBACK;
来源：http://buh.yuxming.cn

[Q66] 行锁查询
来源：http://wde.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xli.uphjek.com

[Q67] 设置隔离级别
来源：http://tzs.fzhhl.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nbb.chenjidiqi.icu

[Q68] 保存点
来源：http://tfa.tian-w.cn

SAVEPOINT sp1;
来源：http://ont.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://hjg.316326.xyz

[Q69] 查看执行计划
来源：http://xml.vqdsnc.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://txe.bjfxy.top

[Q70] 更新统计信息
来源：http://azn.shuidangran.top

ANALYZE TABLE users;
来源：http://axn.yongpay.top

[Q71] 查看建表语句
来源：http://zro.zhaomingkeji.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qdo.xylfe.cn

[Q72] 查看索引
来源：http://ntp.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://vba.hammf.cn

[Q73] 查看表状态
来源：http://kjm.fehbvm.com

SHOW TABLE STATUS LIKE 'users';
来源：http://jop.jinqigufen.top

[Q74] 强制使用索引
来源：http://ikm.gaohongyu789.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wgy.zdqjudy.top

[Q75] 日期格式化
来源：http://mpx.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eca.tarul.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dpp.0kj1m.cn

[Q76] 按天统计
来源：http://mep.nwbrower.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vnl.sjlbkw.cn

[Q77] 时间加减
来源：http://rjz.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dwc.bbcook.cn

[Q78] 当前时间
来源：http://rjf.hesvh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kxi.zhongyouzk.top

[Q79] 字符串拼接
来源：http://ehg.jinqigufen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gbs.guannengcc.top

[Q80] 字符串截取
来源：http://uqz.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rbb.jyoumei.cn

[Q81] 字符串替换
来源：http://sii.snrcjt.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://woz.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://ggu.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kmt.jinqigfzy.top

[Q83] 大小写转换
来源：http://prc.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ptm.xuanzx.com

[Q84] 去除首尾空格
来源：http://oyt.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://fdm.ivvv.top

[Q85] 数值取整
来源：http://arn.hfpthk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ewi.jqgufenzy.top

[Q86] 读取 JSON 字段
来源：http://zjk.hongshengwenyu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pco.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://lbo.ywan-chungtsiang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jkk.jqgfzy.top

[Q88] 行转列（条件聚合）
来源：http://mkv.hesvh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xtd.shangyingyoupin.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tiy.fktsv.cn

[Q89] 判断表是否存在
来源：http://ely.yj20258888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vns.gzhubu.top

[Q90] 生成序号列
来源：http://xgt.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dqg.chenjidiqi.icu

================================================================================
来源：http://mbv.hnxiangtu.top

R. Bash 专题
来源：http://qul.pengpengdd.cyou

================================================================================
来源：http://pos.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://bpt.zdbjq.cn

#!/usr/bin/env bash
来源：http://iqd.yonumen.top

set -euo pipefail
来源：http://jww.52xcode.cn

[R02] 变量赋值与使用
来源：http://jfj.yueranfly.top

name="Tom"; echo "$name"
来源：http://jxs.cdnleiting.top

[R03] 只读变量
来源：http://ilf.vqdsnc.cn

readonly PI=3.14
来源：http://jen.yuxming.cn

[R04] 位置参数
来源：http://mtf.cheryme.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wir.bbcook.cn

[R05] 参数默认值
来源：http://nzk.iojbl.cn

name="${1:-default}"
来源：http://ztu.ybcxt.top

[R06] 判断命令是否存在
来源：http://kar.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mtr.316326.xyz

[R07] if 判断文件
来源：http://dqw.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://whv.hywenlv.cn

[R08] 数值比较
来源：http://qga.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://osd.cucudq.cn

[R09] 字符串比较
来源：http://bef.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tom.jinqigufen.top

[R10] 正则匹配
来源：http://qhb.guowangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tcw.xinyue.icu

[R11] case 多分支
来源：http://udl.jinqigufen.top

case "$1" in
来源：http://jie.jinqigfzy.top

start) echo "启动" ;;
来源：http://ydt.ybcxt.top

stop)  echo "停止" ;;
来源：http://stf.epnwcf.com

*)     echo "未知命令" ;;
来源：http://cab.hesvh.cn

esac
来源：http://axj.zhixingplan.top

[R12] for 遍历文件
来源：http://fsd.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://fuq.iojbl.cn

[R13] for 计数循环
来源：http://xdg.zhaomingkeji.xyz

for i in {1..10}; do echo "$i"; done
来源：http://raw.shuidangran.top

[R14] C 风格 for
来源：http://ynj.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xpg.ydjk.org.cn

[R15] while 逐行读文件
来源：http://ylz.jianghu66.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vtp.gzhubu.top

[R16] until 等待条件
来源：http://hhw.jianghu66.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bcg.guannengcc.top

[R17] 数组定义与取值
来源：http://ufu.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qwf.pengpengdd.cyou

[R18] 遍历数组
来源：http://tef.aibaodan.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zwz.fzhhl.top

[R19] 数组长度
来源：http://ezi.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://rvk.zhoulong.xyz

[R20] 关联数组（字典）
来源：http://fxd.jinqigfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yiu.redwolf501.top

[R21] 字符串长度
来源：http://gke.jinghuilouyu.cn

echo "${#s}"
来源：http://jve.kuanghao11.cn

[R22] 截取子串
来源：http://frm.hnqzz.top

echo "${s:0:5}"
来源：http://kzi.yj20258.top

[R23] 字符串替换
来源：http://zsv.fanxiaobao.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yks.meibo888.top

[R24] 大小写转换
来源：http://opx.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yvj.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://nag.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jrq.jqgufenzy.top

[R26] 命令替换
来源：http://pcn.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://bwr.fanxiaobao.xyz

[R27] 算术展开
来源：http://sca.ppjwa.cn

echo $((1 + 2 * 3))
来源：http://fuu.tianlin.xyz

[R28] 浮点运算
来源：http://abr.zhiwuduotai.top

echo "scale=2; 10/3" | bc
来源：http://ywi.jlsjyb.cn

[R29] 定义函数
来源：http://mda.xuetiantiany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://asn.haohaochexian.top

[R30] 函数返回状态码
来源：http://gwi.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://lys.gzhubu.top

[R31] 局部变量
来源：http://ozt.0kj1m.cn

f() { local x=1; echo "$x"; }
来源：http://dvd.tanke756.top

[R32] 参数个数校验
来源：http://mlx.fengsongda.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sbj.xylfe.cn

[R33] 捕获错误并提示行号
来源：http://htk.shangyingyoupin.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nvt.yj20258.top

[R34] 退出时清理
来源：http://pdb.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://ulu.bbcook.cn

[R35] 后台执行并等待
来源：http://vhj.shzxlz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qoy.guannengcc.top

[R36] 并发执行多个任务
来源：http://ojd.wangdashe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yyn.cqqwz.cn

[R37] 把输出赋给变量
来源：http://dee.sweek.top

files=$(ls -1)
来源：http://css.aizwys.cn

[R38] 管道串联
来源：http://lvn.zhixingplan.top

cat a.txt | grep -i error | wc -l
来源：http://eym.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://rga.jinqigufen.top

cmd > out.log 2>&1
来源：http://sti.zhiwuduotai.top

[R40] 追加写日志
来源：http://vbo.shanyushiyangtech.top

echo "log" >> out.log
来源：http://hok.yangfankeji.com

[R41] 丢弃输出
来源：http://edc.yfazqb.com

cmd >/dev/null 2>&1
来源：http://yyw.xuetiantiany.cn

[R42] 输入重定向
来源：http://oid.hcnkem.com

wc -l < a.txt
来源：http://dek.yangfankeji.com

[R43] 按名字查找文件
来源：http://rrh.smart0.xyz

find . -name "*.log" -type f
来源：http://rta.vqdsnc.cn

[R44] 按修改时间查找
来源：http://rwf.gotoacloud.top

find . -mtime -7 -type f
来源：http://osr.cucudq.cn

[R45] 批量删除
来源：http://nap.yvedp.cn

find . -name "*.tmp" -delete
来源：http://jht.wangdashe.top

[R46] 递归替换文件内容
来源：http://fhe.sufxvd.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wzs.gogol.net.cn

[R47] sed 单行替换
来源：http://skz.aibaodan.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gwf.cashguo.top

[R48] awk 取指定列
来源：http://bwi.fehbvm.com

awk '{print $1, $3}' a.txt
来源：http://mmr.chenlongwang.top

[R49] awk 带条件
来源：http://cnu.feifeiyinyue.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hzb.shangyingyoupin.top

[R50] awk 求和
来源：http://ray.jinghuilouyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ltn.xylfe.cn

[R51] 排序去重取前几
来源：http://giz.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wwh.cdnleiting.top

[R52] 统计行数
来源：http://ajc.wangshuangyany.cn

wc -l a.txt
来源：http://ttd.sjlbkw.cn

[R53] 查看文件头与实时尾
来源：http://wag.hammf.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rjy.dashuyun.cn

[R54] 比较两个文件
来源：http://dtr.tarul.cn

diff a.txt b.txt
来源：http://gij.tarul.cn

[R55] 压缩与解压
来源：http://xbx.vehdjk.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mrs.aibaodan.cn

[R56] 远程拷贝
来源：http://sqh.xinyue.icu

scp file user@host:/path/
来源：http://ezz.jqgfzy.top

[R57] 远程执行命令
来源：http://rqw.jqgfzy.top

ssh user@host 'uptime'
来源：http://njk.jinqigfzy.top

[R58] 下载文件
来源：http://dxd.jinghuilouyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kzw.smart0.xyz

[R59] 发 POST JSON
来源：http://prm.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://otv.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://zgc.tarul.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mut.jianghu66.top

[R61] 磁盘占用
来源：http://uzz.dianchejie.cn

df -h;  du -sh *
来源：http://sxx.vehdjk.com

[R62] 找最占空间的文件
来源：http://poq.zhiwuduotai.top

du -ah . | sort -rh | head -10
来源：http://vpa.zdbjq.cn

[R63] 内存与进程
来源：http://qxp.zhengqikj.top

free -h;  ps aux | grep nginx
来源：http://rpy.hywenlv.cn

[R64] 结束进程
来源：http://irx.daria6918.cn

kill -9 $(pgrep -f app.py)
来源：http://xwx.bjfxy.top

[R65] 查看端口占用
来源：http://vep.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rze.jianghu66.top

[R66] 定时任务
来源：http://evp.chenlongwang.top

crontab -e;  crontab -l
来源：http://urc.aizwys.cn

[R67] 生成随机十六进制串
来源：http://qri.epnwcf.com

openssl rand -hex 16
来源：http://wri.yfazqb.com

[R68] 计算文件校验值
来源：http://biv.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://kkd.chenlongwang.top

[R69] 生成随机密码
来源：http://mhx.vehdjk.com

head -c 16 /dev/urandom | base64
来源：http://cne.hongshengwenyu.top

[R70] 时间戳与互转
来源：http://vox.cashguo.top

date +%s;  date -d @1700000000
来源：http://pcq.yuanzhike.top

[R71] 日期格式化
来源：http://ohb.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fzq.ybcxt.top

[R72] 等待端口就绪
来源：http://amw.yvedp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fuu.meibo888.top

[R73] 分割大日志
来源：http://dfp.redwolf501.top

split -l 1000 big.log part_
来源：http://cus.kuanghao11.cn

[R74] 批量重命名
来源：http://kbc.xingfuxueyuan.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://odg.daria6918.cn

[R75] 导出环境变量
来源：http://zxg.zhaomingkeji.xyz

export PATH="$HOME/bin:$PATH"
来源：http://hmg.hammf.cn

[R76] 使用临时文件
来源：http://ehe.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zua.yuxming.cn

[R77] 读取用户输入
来源：http://tfl.haohaochexian.top

read -rp "请输入: " ans
来源：http://rmf.feifeiyinyue.top

[R78] 交互式菜单
来源：http://kks.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qzm.daxiang520.top

[R79] 解析命令行选项
来源：http://wme.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pcl.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://bpo.ywan-chungtsiang.top

time ./run.sh
来源：http://vck.zhijiandao.cn

================================================================================
来源：http://bxp.jinghuilouyu.cn

S. C / C++ 专题
来源：http://tdd.yongpay.top

================================================================================
来源：http://nri.daxiang520.top

[S01] C：Hello World
来源：http://zwl.jinghuilouyu.cn

#include <stdio.h>
来源：http://fdt.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kky.jinghuilouyu.cn

[S02] C：变量与格式化输出
来源：http://bqa.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://xsn.cqqwz.cn

[S03] C：读入整数
来源：http://pyv.tarul.cn

int x; scanf("%d", &x);
来源：http://fql.jianghu66.top

[S04] C：字符串复制
来源：http://jkw.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://vnk.guowangkeji.top

[S05] C：字符串长度
来源：http://hlm.svipenyu.cn

strlen(s)
来源：http://efo.tanke756.top

[S06] C：字符串比较
来源：http://naq.yueranfly.top

strcmp(a, b) == 0
来源：http://upi.shangyingyoupin.top

[S07] C：数组遍历求和
来源：http://qwx.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gin.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://wyp.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nwn.haohaochexian.top

[S09] C：结构体定义与初始化
来源：http://bnt.tanke756.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://igy.birdmap.top

[S10] C：指针与解引用
来源：http://fwt.daria6918.cn

int *p = &a;  *p = 5;
来源：http://yeg.cucudq.cn

[S11] C：逐行读文件
来源：http://bto.yuxming.cn

FILE *f = fopen("a.txt", "r");
来源：http://mxh.wangshuangyany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://htp.yueranfly.top

fclose(f);
来源：http://gpo.birdmap.top

[S12] C：写文件
来源：http://pex.redwolf501.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jcw.hywenlv.cn

[S13] C：宏定义
来源：http://dee.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kng.chenzaomai.com

[S14] C：枚举
来源：http://ade.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://aeo.fanxiaobao.xyz

[S15] C：类型转换
来源：http://nuu.nanxinkj.top

(double) a / b
来源：http://haj.jiagoushi.top

[S16] C：位操作置位
来源：http://yod.hongshengwenyu.top

x |= (1 << 3);
来源：http://eji.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://ydo.dashuyun.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kyc.uphjek.com

[S18] C：命令行参数
来源：http://mli.hammf.cn

int main(int argc, char **argv)
来源：http://amz.fehbvm.com

[S19] C：快速排序
来源：http://ens.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://fgy.yvedp.cn

[S20] C：二分查找
来源：http://xqe.yueranfly.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ooz.yfazqb.com

[S21] C：字符类别判断
来源：http://oca.vqdsnc.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jup.yueranfly.top

[S22] C：字符串转数字
来源：http://rpe.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://omy.gogol.net.cn

[S23] C：随机数
来源：http://vyr.cqqwz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qhp.uphjek.com

[S24] C：获取本地时间
来源：http://dlm.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qqe.sysykeji.top

[S25] C：内存拷贝
来源：http://ewm.dianchejie.cn

memcpy(dst, src, n);
来源：http://jcx.zhengqikj.top

[S26] C：内存清零
来源：http://uqf.fzhhl.top

memset(a, 0, sizeof a);
来源：http://pff.smart0.xyz

[S27] C：定义常量
来源：http://scw.52xcode.cn

const double PI = 3.14159;
来源：http://cei.tianlin.xyz

[S28] C：静态变量
来源：http://ejg.tarul.cn

static int counter = 0;
来源：http://cqa.fengsongda.top

[S29] C：变参函数
来源：http://rxp.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xqq.sysykeji.top

[S30] C：头文件保护
来源：http://ors.svipenyu.cn

#ifndef X_H
来源：http://smb.ybcxt.top

#define X_H
来源：http://jqa.fanxiaobao.xyz

#endif
来源：http://vqz.wangshuangyany.cn

[S31] C++：Hello World
来源：http://lap.xinyue.icu

#include <iostream>
来源：http://ikv.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://qcb.tian-w.cn

[S32] C++：字符串
来源：http://doq.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://dkl.gotoacloud.top

[S33] C++：vector 增删
来源：http://voc.bjfxy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kus.hfpthk.cn

[S34] C++：遍历 vector
来源：http://xpg.fehbvm.com

for (auto &x : v) { std::cout << x; }
来源：http://fii.zycfv.cn


<!-- 参考信息 -->