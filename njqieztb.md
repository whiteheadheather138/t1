代发 wailian999

[Q63] 开启事务
来源：http://hye.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xcl.c1oappe.top

[Q64] 提交事务
来源：http://spm.zhiwuduotai.top

COMMIT;
来源：http://yjk.chenlongwang.top

[Q65] 回滚事务
来源：http://hto.quarkkingdee.top

ROLLBACK;
来源：http://pwa.andypj.xyz

[Q66] 行锁查询
来源：http://gqk.jqgfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rkn.xylfe.cn

[Q67] 设置隔离级别
来源：http://zci.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lmo.zycfv.cn

[Q68] 保存点
来源：http://xte.xinyue.icu

SAVEPOINT sp1;
来源：http://qmu.yueranfly.top

ROLLBACK TO sp1;
来源：http://jxg.ehwqpu.com

[Q69] 查看执行计划
来源：http://atj.zhijiandao.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://txp.ydzc1.top

[Q70] 更新统计信息
来源：http://wjo.jinqigufen.top

ANALYZE TABLE users;
来源：http://wxk.ydjk.org.cn

[Q71] 查看建表语句
来源：http://hlt.smart0.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://olk.dashuyun.cn

[Q72] 查看索引
来源：http://oxp.bjfxy.top

SHOW INDEX FROM users;
来源：http://vea.shzxlz.cn

[Q73] 查看表状态
来源：http://ukk.shanyushiyangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ttc.yangfankeji.com

[Q74] 强制使用索引
来源：http://teb.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ljk.yj20258.top

[Q75] 日期格式化
来源：http://tyo.yanxiufei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jsh.yuanzhike.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lio.tian-w.cn

[Q76] 按天统计
来源：http://mjf.jqgufenzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gst.pycfn.com

[Q77] 时间加减
来源：http://ufh.zdbjq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dlk.yongpay.top

[Q78] 当前时间
来源：http://nki.dianchejie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vyt.shzxlz.cn

[Q79] 字符串拼接
来源：http://rnw.jinqigufen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://igz.zhiwuduotai.top

[Q80] 字符串截取
来源：http://haj.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gnm.xuanzx.com

[Q81] 字符串替换
来源：http://kbq.sweek.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ecr.fengsongda.top

[Q82] 字符长度与字节长度
来源：http://gcl.fehbvm.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mrs.yfazqb.com

[Q83] 大小写转换
来源：http://day.yj202588.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aeg.tanke756.top

[Q84] 去除首尾空格
来源：http://dor.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://yrf.pengpengdd.cyou

[Q85] 数值取整
来源：http://smi.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://abj.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://exw.ydjk.org.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gbq.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://lui.tanke756.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zsd.vehdjk.com

[Q88] 行转列（条件聚合）
来源：http://kmx.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mgm.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://faq.andypj.xyz

[Q89] 判断表是否存在
来源：http://lhs.jinqigufen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wka.aibaodan.cn

[Q90] 生成序号列
来源：http://whd.jqgufenzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uhx.bbcook.cn

================================================================================
来源：http://cph.chenjidiqi.icu

R. Bash 专题
来源：http://pim.hnqzz.top

================================================================================
来源：http://gxp.bjfxy.top

[R01] shebang 与严格模式
来源：http://whq.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://btm.zdqjudy.top

set -euo pipefail
来源：http://qpk.tanke756.top

[R02] 变量赋值与使用
来源：http://reg.tianlin.xyz

name="Tom"; echo "$name"
来源：http://vvv.sxryk.cn

[R03] 只读变量
来源：http://pxv.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://jhq.ywan-chungtsiang.top

[R04] 位置参数
来源：http://alq.jianghu66.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wws.0kj1m.cn

[R05] 参数默认值
来源：http://fqo.hnqzz.top

name="${1:-default}"
来源：http://ugf.guannengcc.top

[R06] 判断命令是否存在
来源：http://paf.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ypb.hesvh.cn

[R07] if 判断文件
来源：http://vmr.yueranfly.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rqo.dashuyun.cn

[R08] 数值比较
来源：http://lgq.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yhi.hongshengwenyu.top

[R09] 字符串比较
来源：http://iia.zdbjq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sma.kuanghao11.cn

[R10] 正则匹配
来源：http://yik.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hca.tianlin.xyz

[R11] case 多分支
来源：http://vbx.yangfankeji.com

case "$1" in
来源：http://cnr.9152youxi.cn

start) echo "启动" ;;
来源：http://pfo.smart0.xyz

stop)  echo "停止" ;;
来源：http://tto.pycfn.com

*)     echo "未知命令" ;;
来源：http://sug.shanyushiyangtech.top

esac
来源：http://mks.ybcxt.top

[R12] for 遍历文件
来源：http://prs.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://edl.chenlongwang.top

[R13] for 计数循环
来源：http://wvm.sysykeji.top

for i in {1..10}; do echo "$i"; done
来源：http://vrp.fengsongda.top

[R14] C 风格 for
来源：http://rzd.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ste.xziqi.cn

[R15] while 逐行读文件
来源：http://ris.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ffs.c1oappe.top

[R16] until 等待条件
来源：http://wlv.nwbrower.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://khb.hcnkem.com

[R17] 数组定义与取值
来源：http://gpj.hongshengwenyu.top

arr=(a b c); echo "${arr[0]}"
来源：http://bps.hnxiangtu.top

[R18] 遍历数组
来源：http://qur.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lau.jlsjyb.cn

[R19] 数组长度
来源：http://mpr.hcnkem.com

echo "${#arr[@]}"
来源：http://szn.chenzaomai.com

[R20] 关联数组（字典）
来源：http://ega.hfpthk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wrn.daria6918.cn

[R21] 字符串长度
来源：http://dlo.c1oappe.top

echo "${#s}"
来源：http://qyp.dashuyun.cn

[R22] 截取子串
来源：http://hag.gotoacloud.top

echo "${s:0:5}"
来源：http://kqk.zhixingplan.top

[R23] 字符串替换
来源：http://ywi.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fhu.aizwys.cn

[R24] 大小写转换
来源：http://ptq.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://jmf.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://ajg.iojbl.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fpd.wangdashe.top

[R26] 命令替换
来源：http://pqp.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://gay.tian-w.cn

[R27] 算术展开
来源：http://odq.yj202588.top

echo $((1 + 2 * 3))
来源：http://oin.316326.xyz

[R28] 浮点运算
来源：http://vbg.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://qfs.shanyushiyangkeji.top

[R29] 定义函数
来源：http://xfv.sysykeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bhc.wangdashe.top

[R30] 函数返回状态码
来源：http://fra.birdmap.top

f() { return 0; }; f || echo "失败了"
来源：http://tcy.hammf.cn

[R31] 局部变量
来源：http://iaw.shzxlz.cn

f() { local x=1; echo "$x"; }
来源：http://gkx.gzhubu.top

[R32] 参数个数校验
来源：http://bch.ywan-chungtsiang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kdm.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://vtp.yanxiufei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wph.jqgfzy.top

[R34] 退出时清理
来源：http://ful.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://cnu.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://mzh.pengpengdd.cyou

sleep 5 & pid=$!; wait "$pid"
来源：http://npd.dianchejie.cn

[R36] 并发执行多个任务
来源：http://gjq.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ceu.shzxlz.cn

[R37] 把输出赋给变量
来源：http://jia.chenzaomai.com

files=$(ls -1)
来源：http://khi.hongshengwenyu.top

[R38] 管道串联
来源：http://lti.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://ljn.jqgufenzy.top

[R39] 重定向标准输出与错误
来源：http://qqy.kuanghao11.cn

cmd > out.log 2>&1
来源：http://npn.gogol.net.cn

[R40] 追加写日志
来源：http://eqs.sweek.top

echo "log" >> out.log
来源：http://rva.zhengqikj.top

[R41] 丢弃输出
来源：http://zwc.fzhhl.top

cmd >/dev/null 2>&1
来源：http://nek.svipenyu.cn

[R42] 输入重定向
来源：http://sct.daxiang520.top

wc -l < a.txt
来源：http://cjw.yongpay.top

[R43] 按名字查找文件
来源：http://ift.epnwcf.com

find . -name "*.log" -type f
来源：http://kpt.xinyue.icu

[R44] 按修改时间查找
来源：http://lqm.shzxlz.cn

find . -mtime -7 -type f
来源：http://gtt.9152youxi.cn

[R45] 批量删除
来源：http://azj.chenjidiqi.icu

find . -name "*.tmp" -delete
来源：http://urw.jyoumei.cn

[R46] 递归替换文件内容
来源：http://mlx.jiagoushi.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vkv.hywenlv.cn

[R47] sed 单行替换
来源：http://ide.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pbt.shzxlz.cn

[R48] awk 取指定列
来源：http://aic.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://vgn.zycfv.cn

[R49] awk 带条件
来源：http://mnr.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ccs.sjlbkw.cn

[R50] awk 求和
来源：http://gqu.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://kuk.gotoacloud.top

[R51] 排序去重取前几
来源：http://sob.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://azf.feifeiyinyue.top

[R52] 统计行数
来源：http://eti.jqgfzy.top

wc -l a.txt
来源：http://upv.hywenlv.cn

[R53] 查看文件头与实时尾
来源：http://qkb.316326.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zja.dashuyun.cn

[R54] 比较两个文件
来源：http://pwu.316326.xyz

diff a.txt b.txt
来源：http://qaj.yj20258888.top

[R55] 压缩与解压
来源：http://mhs.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://suw.fzhhl.top

[R56] 远程拷贝
来源：http://hyi.jyoumei.cn

scp file user@host:/path/
来源：http://gsi.yonumen.top

[R57] 远程执行命令
来源：http://sut.mhx1999.top

ssh user@host 'uptime'
来源：http://xgd.hnqzz.top

[R58] 下载文件
来源：http://noi.andypj.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://con.jinqigufen.top

[R59] 发 POST JSON
来源：http://blo.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://foa.cashguo.top

[R60] 只看 HTTP 状态码
来源：http://gur.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jsh.cucudq.cn

[R61] 磁盘占用
来源：http://qcg.xuanzx.com

df -h;  du -sh *
来源：http://bxi.xinyue.icu

[R62] 找最占空间的文件
来源：http://mhh.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://tbw.yfazqb.com

[R63] 内存与进程
来源：http://pxl.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://rqs.gzhubu.top

[R64] 结束进程
来源：http://pxl.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://mvt.shuidangran.top

[R65] 查看端口占用
来源：http://bsq.shanyushiyangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qnh.ydjk.org.cn

[R66] 定时任务
来源：http://nmj.fktsv.cn

crontab -e;  crontab -l
来源：http://xwt.andypj.xyz

[R67] 生成随机十六进制串
来源：http://zto.hcnkem.com

openssl rand -hex 16
来源：http://ajg.hysaishi.cn

[R68] 计算文件校验值
来源：http://rwt.daria6918.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dhb.dashuyun.cn

[R69] 生成随机密码
来源：http://ccq.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://bsq.chenzaomai.com

[R70] 时间戳与互转
来源：http://wfd.fehbvm.com

date +%s;  date -d @1700000000
来源：http://xez.gotoacloud.top

[R71] 日期格式化
来源：http://gfc.zhongyouzk.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fpj.fktsv.cn

[R72] 等待端口就绪
来源：http://bhd.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hzj.fzhhl.top

[R73] 分割大日志
来源：http://fsu.zhongyouzk.top

split -l 1000 big.log part_
来源：http://wzh.guowangkeji.top

[R74] 批量重命名
来源：http://xjm.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zso.sjlbkw.cn

[R75] 导出环境变量
来源：http://uig.xingfuxueyuan.xyz

export PATH="$HOME/bin:$PATH"
来源：http://osh.andypj.xyz

[R76] 使用临时文件
来源：http://joz.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rye.jyoumei.cn

[R77] 读取用户输入
来源：http://pzt.sxryk.cn

read -rp "请输入: " ans
来源：http://zqt.jinghuilouyu.cn

[R78] 交互式菜单
来源：http://fhr.smart0.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://jrk.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://ivf.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://urj.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://vcq.feifeiyinyue.top

time ./run.sh
来源：http://bnt.xylfe.cn

================================================================================
来源：http://vqm.kuanghao11.cn

S. C / C++ 专题
来源：http://iju.sufxvd.cn

================================================================================
来源：http://meb.pycfn.com

[S01] C：Hello World
来源：http://bmf.zhongyouzk.top

#include <stdio.h>
来源：http://yas.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://usj.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://kcg.haohaochexian.top

int a = 10; printf("%d\n", a);
来源：http://ilj.hywenlv.cn

[S03] C：读入整数
来源：http://vqi.sysykeji.top

int x; scanf("%d", &x);
来源：http://znt.zdbjq.cn

[S04] C：字符串复制
来源：http://zif.hfpthk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lin.guannengcc.top

[S05] C：字符串长度
来源：http://liw.zdqjudy.top

strlen(s)
来源：http://kif.zdqjudy.top

[S06] C：字符串比较
来源：http://ozg.snrcjt.cn

strcmp(a, b) == 0
来源：http://hzx.yueranfly.top

[S07] C：数组遍历求和
来源：http://ddq.redwolf501.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sgb.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://jhn.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qhd.aibaodan.cn

[S09] C：结构体定义与初始化
来源：http://jzg.tianlin.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xpl.zhixingplan.top

[S10] C：指针与解引用
来源：http://nnj.yj20258.top

int *p = &a;  *p = 5;
来源：http://nuj.cqqwz.cn

[S11] C：逐行读文件
来源：http://uda.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://ugf.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ext.fanxiaobao.xyz

fclose(f);
来源：http://dsl.hcnkem.com

[S12] C：写文件
来源：http://fvy.fengsongda.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vso.yonumen.top

[S13] C：宏定义
来源：http://tmy.sjlbkw.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cjn.xziqi.cn

[S14] C：枚举
来源：http://ihw.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://wim.zhixingplan.top

[S15] C：类型转换
来源：http://xuj.jinqigufen.top

(double) a / b
来源：http://bgp.hfpthk.cn

[S16] C：位操作置位
来源：http://wqm.meibo888.top

x |= (1 << 3);
来源：http://ejp.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://xix.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uzy.wangshuangyany.cn

[S18] C：命令行参数
来源：http://zix.zhoulong.xyz

int main(int argc, char **argv)
来源：http://uvf.hywenlv.cn

[S19] C：快速排序
来源：http://eqm.hfpthk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zgf.tian-w.cn

[S20] C：二分查找
来源：http://bww.pengpengdd.cyou

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xka.birdmap.top

[S21] C：字符类别判断
来源：http://gme.yfazqb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tpf.aizwys.cn

[S22] C：字符串转数字
来源：http://kdi.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xhn.hesvh.cn

[S23] C：随机数
来源：http://mcj.yangfankeji.com

srand(time(NULL));  int r = rand() % 100;
来源：http://kbq.ivvv.top

[S24] C：获取本地时间
来源：http://gky.daria6918.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eev.tianlin.xyz

[S25] C：内存拷贝
来源：http://sch.vqdsnc.cn

memcpy(dst, src, n);
来源：http://wcj.zhoulong.xyz

[S26] C：内存清零
来源：http://zsy.nwbrower.top

memset(a, 0, sizeof a);
来源：http://pwu.hongshengwenyu.top

[S27] C：定义常量
来源：http://xnr.yuxming.cn

const double PI = 3.14159;
来源：http://fgo.svipenyu.cn

[S28] C：静态变量
来源：http://ewn.0kj1m.cn

static int counter = 0;
来源：http://bfs.yvedp.cn

[S29] C：变参函数
来源：http://wvs.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qrb.ctjpmb.com

[S30] C：头文件保护
来源：http://ozt.feifeiyinyue.top

#ifndef X_H
来源：http://ble.yuanzhike.top

#define X_H
来源：http://cku.hysaishi.cn

#endif
来源：http://hlw.tian-w.cn

[S31] C++：Hello World
来源：http://sic.hywenlv.cn

#include <iostream>
来源：http://zyu.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://mxg.fktsv.cn

[S32] C++：字符串
来源：http://dix.redwolf501.top

std::string s = "hi";  s += "!";
来源：http://mop.yfazqb.com


<!-- 参考信息 -->