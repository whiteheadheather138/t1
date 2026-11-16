代发 wailian999

[Q61] 移动平均
来源：http://pcz.hesvh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://piw.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://yiw.cashguo.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://boz.ywan-chungtsiang.top

[Q63] 开启事务
来源：http://zaq.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pvx.zhixingplan.top

[Q64] 提交事务
来源：http://pom.hnxiangtu.top

COMMIT;
来源：http://dib.bbcook.cn

[Q65] 回滚事务
来源：http://lsy.chenzaomai.com

ROLLBACK;
来源：http://bao.cucudq.cn

[Q66] 行锁查询
来源：http://jyo.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kwo.xziqi.cn

[Q67] 设置隔离级别
来源：http://ove.hnxiangtu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://igo.hysaishi.cn

[Q68] 保存点
来源：http://sus.sweek.top

SAVEPOINT sp1;
来源：http://aqh.ehwqpu.com

ROLLBACK TO sp1;
来源：http://iut.snrcjt.cn

[Q69] 查看执行计划
来源：http://hla.zhijiandao.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qkb.aizwys.cn

[Q70] 更新统计信息
来源：http://ihg.redwolf501.top

ANALYZE TABLE users;
来源：http://onb.fzhhl.top

[Q71] 查看建表语句
来源：http://vom.meibo888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ysq.0kj1m.cn

[Q72] 查看索引
来源：http://iea.feifeiyinyue.top

SHOW INDEX FROM users;
来源：http://xlx.zhongyouzk.top

[Q73] 查看表状态
来源：http://rdg.yuanzhike.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tzd.sweek.top

[Q74] 强制使用索引
来源：http://mhc.daxiang520.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yxa.hysaishi.cn

[Q75] 日期格式化
来源：http://tmb.hongshengwenyu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fha.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://omz.meibo888.top

[Q76] 按天统计
来源：http://egy.hfpthk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wyj.sxryk.cn

[Q77] 时间加减
来源：http://dsa.yangfankeji.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vki.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://lxw.zhiwuduotai.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jck.daria6918.cn

[Q79] 字符串拼接
来源：http://sap.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sez.tarul.cn

[Q80] 字符串截取
来源：http://zxk.ehwqpu.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rey.gogol.net.cn

[Q81] 字符串替换
来源：http://jgm.yuanzhike.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vss.tianlin.xyz

[Q82] 字符长度与字节长度
来源：http://nqr.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vnk.sjlbkw.cn

[Q83] 大小写转换
来源：http://nvq.jinyuanbaomall.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bwb.yueranfly.top

[Q84] 去除首尾空格
来源：http://khv.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://bkf.yonumen.top

[Q85] 数值取整
来源：http://xyj.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vaq.yonumen.top

[Q86] 读取 JSON 字段
来源：http://uwk.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://okv.xingfuxueyuan.xyz

[Q87] JSON 字段做条件
来源：http://tod.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mvs.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://jvp.epnwcf.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gsm.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xqd.gotoacloud.top

[Q89] 判断表是否存在
来源：http://pjq.yj20258888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fem.dianchejie.cn

[Q90] 生成序号列
来源：http://svu.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://phj.shuidangran.top

================================================================================
来源：http://gjp.52xcode.cn

R. Bash 专题
来源：http://ley.zhixingplan.top

================================================================================
来源：http://brl.hysaishi.cn

[R01] shebang 与严格模式
来源：http://vny.xylfe.cn

#!/usr/bin/env bash
来源：http://zwg.zdqjudy.top

set -euo pipefail
来源：http://mqh.tianlin.xyz

[R02] 变量赋值与使用
来源：http://bxx.gaohongyu789.top

name="Tom"; echo "$name"
来源：http://plp.yanxiufei.cn

[R03] 只读变量
来源：http://hgz.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://sbh.jqgfzy.top

[R04] 位置参数
来源：http://mde.vqdsnc.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lms.meibo888.top

[R05] 参数默认值
来源：http://dhb.meibo888.top

name="${1:-default}"
来源：http://xxd.tianlin.xyz

[R06] 判断命令是否存在
来源：http://fbt.redwolf501.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ixf.yangfankeji.com

[R07] if 判断文件
来源：http://han.daria6918.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gnh.hywenlv.cn

[R08] 数值比较
来源：http://aua.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://vcz.guannengcc.top

[R09] 字符串比较
来源：http://duf.shuidangran.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kys.gogol.net.cn

[R10] 正则匹配
来源：http://wix.cqqwz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vmi.sufxvd.cn

[R11] case 多分支
来源：http://rmd.dashuyun.cn

case "$1" in
来源：http://obc.fktsv.cn

start) echo "启动" ;;
来源：http://dpk.shangyingyoupin.top

stop)  echo "停止" ;;
来源：http://tau.tian-w.cn

*)     echo "未知命令" ;;
来源：http://bet.shzxlz.cn

esac
来源：http://peu.yangfankeji.com

[R12] for 遍历文件
来源：http://vsn.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://sio.zhaomingkeji.xyz

[R13] for 计数循环
来源：http://wds.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://wcn.bjfxy.top

[R14] C 风格 for
来源：http://ayf.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hsg.xylfe.cn

[R15] while 逐行读文件
来源：http://ake.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xon.chenzaomai.com

[R16] until 等待条件
来源：http://anf.ctjpmb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oss.yonumen.top

[R17] 数组定义与取值
来源：http://spp.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://gsz.shzxlz.cn

[R18] 遍历数组
来源：http://jvh.iojbl.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zgz.yanxiufei.cn

[R19] 数组长度
来源：http://fdi.hnxiangtu.top

echo "${#arr[@]}"
来源：http://wgq.hysaishi.cn

[R20] 关联数组（字典）
来源：http://rwn.epnwcf.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xcq.kuanghao11.cn

[R21] 字符串长度
来源：http://cje.jiagoushi.top

echo "${#s}"
来源：http://prh.hfpthk.cn

[R22] 截取子串
来源：http://luo.xuetiantiany.cn

echo "${s:0:5}"
来源：http://ind.hcnkem.com

[R23] 字符串替换
来源：http://oze.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://csk.yongpay.top

[R24] 大小写转换
来源：http://rlm.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://qal.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://mry.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://omk.jinyuanbaomall.cn

[R26] 命令替换
来源：http://grq.hnqzz.top

now=$(date +%F); echo "$now"
来源：http://hqd.yongpay.top

[R27] 算术展开
来源：http://xns.wangdashe.top

echo $((1 + 2 * 3))
来源：http://buz.jinyuanbaomall.cn

[R28] 浮点运算
来源：http://bhn.aibaodan.cn

echo "scale=2; 10/3" | bc
来源：http://qmr.sxryk.cn

[R29] 定义函数
来源：http://jax.nanxinkj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xsx.yongpay.top

[R30] 函数返回状态码
来源：http://jpq.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://bxm.aizwys.cn

[R31] 局部变量
来源：http://rdb.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://xsf.jqgufenzy.top

[R32] 参数个数校验
来源：http://rfy.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://isr.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://ahh.jinqigfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ojo.316326.xyz

[R34] 退出时清理
来源：http://yyd.gzhubu.top

trap 'rm -f "$tmp"' EXIT
来源：http://cww.snrcjt.cn

[R35] 后台执行并等待
来源：http://byw.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://opu.pengpengdd.cyou

[R36] 并发执行多个任务
来源：http://izg.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fob.pycfn.com

[R37] 把输出赋给变量
来源：http://atf.ydjk.org.cn

files=$(ls -1)
来源：http://kyn.zhiwuduotai.top

[R38] 管道串联
来源：http://nni.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://pua.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://pjw.snrcjt.cn

cmd > out.log 2>&1
来源：http://pyc.zhongyouzk.top

[R40] 追加写日志
来源：http://oev.wangdashe.top

echo "log" >> out.log
来源：http://lku.bbcook.cn

[R41] 丢弃输出
来源：http://xif.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://xru.xziqi.cn

[R42] 输入重定向
来源：http://gyh.zhengqikj.top

wc -l < a.txt
来源：http://fos.hfpthk.cn

[R43] 按名字查找文件
来源：http://kcp.xziqi.cn

find . -name "*.log" -type f
来源：http://jlz.daria6918.cn

[R44] 按修改时间查找
来源：http://jtd.svipenyu.cn

find . -mtime -7 -type f
来源：http://xug.jinqigufen.top

[R45] 批量删除
来源：http://idn.feifeiyinyue.top

find . -name "*.tmp" -delete
来源：http://ywf.wangdashe.top

[R46] 递归替换文件内容
来源：http://smt.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uhx.vqdsnc.cn

[R47] sed 单行替换
来源：http://vba.ctjpmb.com

sed -i 's/foo/bar/g' a.txt
来源：http://qdg.tianlin.xyz

[R48] awk 取指定列
来源：http://hmo.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://bat.fehbvm.com

[R49] awk 带条件
来源：http://vep.yj20258888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://djs.snrcjt.cn

[R50] awk 求和
来源：http://lcs.cucudq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jjs.hnxiangtu.top

[R51] 排序去重取前几
来源：http://wxv.nanxuanxn.top

sort a.txt | uniq -c | sort -rn | head
来源：http://prm.jinyuanbaomall.cn

[R52] 统计行数
来源：http://qmm.yongpay.top

wc -l a.txt
来源：http://czg.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://xgw.hywenlv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://atf.shanyushiyangtech.top

[R54] 比较两个文件
来源：http://jrm.aibaodan.cn

diff a.txt b.txt
来源：http://nap.vqdsnc.cn

[R55] 压缩与解压
来源：http://fch.wangshuangyany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fnj.hfpthk.cn

[R56] 远程拷贝
来源：http://vfb.pengpengdd.cyou

scp file user@host:/path/
来源：http://bmu.52xcode.cn

[R57] 远程执行命令
来源：http://req.ydzc1.top

ssh user@host 'uptime'
来源：http://xzb.daria6918.cn

[R58] 下载文件
来源：http://mky.meibo888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tlg.nwbrower.top

[R59] 发 POST JSON
来源：http://xxh.gotoacloud.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ipx.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://way.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qhm.meibo888.top

[R61] 磁盘占用
来源：http://kjb.nanxuanxn.top

df -h;  du -sh *
来源：http://srs.jqgfzy.top

[R62] 找最占空间的文件
来源：http://nka.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://yvg.pycfn.com

[R63] 内存与进程
来源：http://utj.zhongyouzk.top

free -h;  ps aux | grep nginx
来源：http://sgm.yueranfly.top

[R64] 结束进程
来源：http://lth.smart0.xyz

kill -9 $(pgrep -f app.py)
来源：http://ake.xylfe.cn

[R65] 查看端口占用
来源：http://kxt.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fah.andypj.xyz

[R66] 定时任务
来源：http://jji.uphjek.com

crontab -e;  crontab -l
来源：http://mij.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://cal.wangshuangyany.cn

openssl rand -hex 16
来源：http://lzj.zhijiandao.cn

[R68] 计算文件校验值
来源：http://dhd.yfazqb.com

sha256sum a.txt;  md5sum a.txt
来源：http://rye.epnwcf.com

[R69] 生成随机密码
来源：http://eep.cashguo.top

head -c 16 /dev/urandom | base64
来源：http://pyb.jlsjyb.cn

[R70] 时间戳与互转
来源：http://yce.shanyushiyangtech.top

date +%s;  date -d @1700000000
来源：http://eis.aibaodan.cn

[R71] 日期格式化
来源：http://wlr.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://eef.ybcxt.top

[R72] 等待端口就绪
来源：http://jlg.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://iju.svipenyu.cn

[R73] 分割大日志
来源：http://rbm.xuanzx.com

split -l 1000 big.log part_
来源：http://ufx.hesvh.cn

[R74] 批量重命名
来源：http://joi.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ohb.ydjk.org.cn

[R75] 导出环境变量
来源：http://gip.sweek.top

export PATH="$HOME/bin:$PATH"
来源：http://rso.ehwqpu.com

[R76] 使用临时文件
来源：http://rro.fktsv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yfe.ppjwa.cn

[R77] 读取用户输入
来源：http://lgv.birdmap.top

read -rp "请输入: " ans
来源：http://jdp.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://ccx.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ytg.ydzc1.top

[R79] 解析命令行选项
来源：http://ajk.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blf.yfazqb.com

[R80] 查看脚本执行耗时
来源：http://tso.daria6918.cn

time ./run.sh
来源：http://xvy.xingfuxueyuan.xyz

================================================================================
来源：http://gib.wangshuangyany.cn

S. C / C++ 专题
来源：http://gmm.yuanzhike.top

================================================================================
来源：http://oog.tarul.cn

[S01] C：Hello World
来源：http://nsx.cheryme.top

#include <stdio.h>
来源：http://qpu.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://klh.hnqzz.top

[S02] C：变量与格式化输出
来源：http://tub.jqgufenzy.top

int a = 10; printf("%d\n", a);
来源：http://ddc.ehwqpu.com

[S03] C：读入整数
来源：http://tsf.tianlin.xyz

int x; scanf("%d", &x);
来源：http://qpp.zhijiandao.cn

[S04] C：字符串复制
来源：http://mdv.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://gqr.hcnkem.com

[S05] C：字符串长度
来源：http://sds.zhaomingkeji.xyz

strlen(s)
来源：http://loh.ydzc1.top

[S06] C：字符串比较
来源：http://jns.jianghu66.top

strcmp(a, b) == 0
来源：http://uce.aizwys.cn

[S07] C：数组遍历求和
来源：http://lwj.tarul.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yaq.dashuyun.cn

[S08] C：动态内存分配与释放
来源：http://djn.jqgfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cjw.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://uvz.jqgufenzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hpw.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://svi.cucudq.cn

int *p = &a;  *p = 5;
来源：http://euc.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://ehd.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://und.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fni.wangshuangyany.cn

fclose(f);
来源：http://jva.yonumen.top

[S12] C：写文件
来源：http://edw.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eum.tarul.cn

[S13] C：宏定义
来源：http://bwi.sxryk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cui.xuetiantiany.cn

[S14] C：枚举
来源：http://zlb.yuanzhike.top

enum Color { RED, GREEN, BLUE };
来源：http://eac.dashuyun.cn

[S15] C：类型转换
来源：http://vdg.ehwqpu.com

(double) a / b
来源：http://xcu.jqgufenzy.top

[S16] C：位操作置位
来源：http://ewl.bjfxy.top

x |= (1 << 3);
来源：http://dcx.jinghuilouyu.cn

[S17] C：安全拼接字符串
来源：http://hqy.jqgufenzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cjx.hnxiangtu.top

[S18] C：命令行参数
来源：http://saf.fengsongda.top

int main(int argc, char **argv)
来源：http://dpn.iojbl.cn

[S19] C：快速排序
来源：http://nck.svipenyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jju.gzhubu.top

[S20] C：二分查找
来源：http://ycz.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tyd.jyoumei.cn

[S21] C：字符类别判断
来源：http://emr.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lat.xziqi.cn

[S22] C：字符串转数字
来源：http://qwz.yanxiufei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rkl.chenjidiqi.icu

[S23] C：随机数
来源：http://bfu.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mfq.fzhhl.top

[S24] C：获取本地时间
来源：http://sik.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://whc.cucudq.cn

[S25] C：内存拷贝
来源：http://szz.aizwys.cn

memcpy(dst, src, n);
来源：http://waq.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://nyu.9152youxi.cn

memset(a, 0, sizeof a);
来源：http://wyo.andypj.xyz

[S27] C：定义常量
来源：http://hvd.daxiang520.top

const double PI = 3.14159;
来源：http://krj.hammf.cn

[S28] C：静态变量
来源：http://cub.jyoumei.cn

static int counter = 0;
来源：http://fvq.dianchejie.cn

[S29] C：变参函数
来源：http://ldz.yj20258.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://khn.guannengcc.top

[S30] C：头文件保护
来源：http://uic.nanxuanxn.top

#ifndef X_H
来源：http://wdf.cdnleiting.top

#define X_H
来源：http://cmu.haohaochexian.top

#endif
来源：http://tjq.hesvh.cn

[S31] C++：Hello World
来源：http://pyx.yj20258.top


<!-- 参考信息 -->