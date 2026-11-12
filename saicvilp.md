代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://grr.ctjpmb.com

[Q54] 清空表
来源：http://zke.xuetiantiany.cn

TRUNCATE TABLE logs;
来源：http://wuk.yueranfly.top

[Q55] 排名（并列占位）
来源：http://vuk.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ufy.ywan-chungtsiang.top

[Q56] 密集排名（并列不占位）
来源：http://qhr.fktsv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nqo.zhengqikj.top

[Q57] 行号
来源：http://eig.mhx1999.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lkk.zhixingplan.top

[Q58] 累计求和
来源：http://gvy.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://esg.mhx1999.top

[Q59] 分组内累计
来源：http://dpi.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://snd.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://cgo.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yjw.zdbjq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pyb.ydzc1.top

[Q61] 移动平均
来源：http://nto.yj202588.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pke.9152youxi.cn

[Q62] 分组占比
来源：http://mgu.nanxinkj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ebu.zhiwuduotai.top

[Q63] 开启事务
来源：http://lyr.sweek.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dvs.zdqjudy.top

[Q64] 提交事务
来源：http://jcz.chenjidiqi.icu

COMMIT;
来源：http://uod.fktsv.cn

[Q65] 回滚事务
来源：http://cea.xylfe.cn

ROLLBACK;
来源：http://ytc.tarul.cn

[Q66] 行锁查询
来源：http://reu.uphjek.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tki.jianghu66.top

[Q67] 设置隔离级别
来源：http://uaj.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gnh.guannengcc.top

[Q68] 保存点
来源：http://leu.ydzc1.top

SAVEPOINT sp1;
来源：http://fpp.jqgfzy.top

ROLLBACK TO sp1;
来源：http://ugb.svipenyu.cn

[Q69] 查看执行计划
来源：http://dxo.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hmv.daxiang520.top

[Q70] 更新统计信息
来源：http://qjv.yonumen.top

ANALYZE TABLE users;
来源：http://zja.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://qks.mhx1999.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lvj.sjlbkw.cn

[Q72] 查看索引
来源：http://xua.jinqigufen.top

SHOW INDEX FROM users;
来源：http://eax.zhoulong.xyz

[Q73] 查看表状态
来源：http://cth.hammf.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dsc.nwbrower.top

[Q74] 强制使用索引
来源：http://god.ehwqpu.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hgn.zhijiandao.cn

[Q75] 日期格式化
来源：http://epv.yj202588.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zpb.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dgx.aizwys.cn

[Q76] 按天统计
来源：http://iix.jlsjyb.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ich.yanxiufei.cn

[Q77] 时间加减
来源：http://azg.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qti.aibaodan.cn

[Q78] 当前时间
来源：http://hre.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jzk.tianlin.xyz

[Q79] 字符串拼接
来源：http://rhg.aizwys.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pgw.cdnleiting.top

[Q80] 字符串截取
来源：http://kjr.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qbj.sweek.top

[Q81] 字符串替换
来源：http://xud.ppjwa.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://eho.yanxiufei.cn

[Q82] 字符长度与字节长度
来源：http://dbf.jianghu66.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ofa.havefunace.top

[Q83] 大小写转换
来源：http://lot.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qoc.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://lrz.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://ktz.shzxlz.cn

[Q85] 数值取整
来源：http://caa.xuetiantiany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lqh.hywenlv.cn

[Q86] 读取 JSON 字段
来源：http://qle.hysaishi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://myq.tarul.cn

[Q87] JSON 字段做条件
来源：http://rpd.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rjh.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://ihn.uphjek.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uqz.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sdy.jinqigufen.top

[Q89] 判断表是否存在
来源：http://tmz.zhixingplan.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://whi.c1oappe.top

[Q90] 生成序号列
来源：http://nsc.yfazqb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jdl.xuetiantiany.cn

================================================================================
来源：http://jjl.daria6918.cn

R. Bash 专题
来源：http://nbx.ivvv.top

================================================================================
来源：http://rrs.9152youxi.cn

[R01] shebang 与严格模式
来源：http://lzm.yuanzhike.top

#!/usr/bin/env bash
来源：http://qgb.gogol.net.cn

set -euo pipefail
来源：http://uxc.tanke756.top

[R02] 变量赋值与使用
来源：http://wyq.shuidangran.top

name="Tom"; echo "$name"
来源：http://pet.hywenlv.cn

[R03] 只读变量
来源：http://ysy.quarkkingdee.top

readonly PI=3.14
来源：http://nva.hnxiangtu.top

[R04] 位置参数
来源：http://cxt.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cfo.zhaomingkeji.xyz

[R05] 参数默认值
来源：http://fyv.jinyuanbaomall.cn

name="${1:-default}"
来源：http://mjq.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://eir.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kys.jinyuanbaomall.cn

[R07] if 判断文件
来源：http://nhf.gotoacloud.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bjb.vqdsnc.cn

[R08] 数值比较
来源：http://bnf.hammf.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iun.cqqwz.cn

[R09] 字符串比较
来源：http://xzp.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mmd.sweek.top

[R10] 正则匹配
来源：http://mjk.shanyushiyangtech.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yjd.chenjidiqi.icu

[R11] case 多分支
来源：http://vzx.tarul.cn

case "$1" in
来源：http://hsl.gaohongyu789.top

start) echo "启动" ;;
来源：http://xbg.xziqi.cn

stop)  echo "停止" ;;
来源：http://ofw.jinghuilouyu.cn

*)     echo "未知命令" ;;
来源：http://mzi.zhongyouzk.top

esac
来源：http://mhi.jyoumei.cn

[R12] for 遍历文件
来源：http://lgg.9152youxi.cn

for f in *.txt; do echo "$f"; done
来源：http://edk.ehwqpu.com

[R13] for 计数循环
来源：http://kug.ydjk.org.cn

for i in {1..10}; do echo "$i"; done
来源：http://bcv.cucudq.cn

[R14] C 风格 for
来源：http://gas.hongshengwenyu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://otr.yonumen.top

[R15] while 逐行读文件
来源：http://jpa.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gez.zdqjudy.top

[R16] until 等待条件
来源：http://jep.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://frn.jinqigfzy.top

[R17] 数组定义与取值
来源：http://xfs.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://vfd.tanke756.top

[R18] 遍历数组
来源：http://rra.daria6918.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fva.gotoacloud.top

[R19] 数组长度
来源：http://npi.fktsv.cn

echo "${#arr[@]}"
来源：http://mwv.ctjpmb.com

[R20] 关联数组（字典）
来源：http://bpn.daxiang520.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dzp.sufxvd.cn

[R21] 字符串长度
来源：http://nne.cheryme.top

echo "${#s}"
来源：http://yao.sufxvd.cn

[R22] 截取子串
来源：http://zjd.dianchejie.cn

echo "${s:0:5}"
来源：http://rnm.guannengcc.top

[R23] 字符串替换
来源：http://axn.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ojn.ctjpmb.com

[R24] 大小写转换
来源：http://dpx.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nbl.0kj1m.cn

[R25] 去后缀 / 去前缀
来源：http://jwk.tanke756.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hqb.dianchejie.cn

[R26] 命令替换
来源：http://jpi.ivvv.top

now=$(date +%F); echo "$now"
来源：http://fsr.yongpay.top

[R27] 算术展开
来源：http://zgc.zhengqikj.top

echo $((1 + 2 * 3))
来源：http://kza.yongpay.top

[R28] 浮点运算
来源：http://lfn.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://nrn.cheryme.top

[R29] 定义函数
来源：http://gqv.havefunace.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xzc.shuidangran.top

[R30] 函数返回状态码
来源：http://miv.sxryk.cn

f() { return 0; }; f || echo "失败了"
来源：http://cmq.c1oappe.top

[R31] 局部变量
来源：http://tkc.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://szm.zhixingplan.top

[R32] 参数个数校验
来源：http://uoq.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jyd.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://zbs.316326.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wur.shanyushiyangtech.top

[R34] 退出时清理
来源：http://qox.guowangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://oen.yongpay.top

[R35] 后台执行并等待
来源：http://jmj.zhijiandao.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://orq.feifeiyinyue.top

[R36] 并发执行多个任务
来源：http://krk.xuetiantiany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://daz.gaohongyu789.top

[R37] 把输出赋给变量
来源：http://lbn.guowangkeji.top

files=$(ls -1)
来源：http://dmg.zhongyouzk.top

[R38] 管道串联
来源：http://fvc.jlsjyb.cn

cat a.txt | grep -i error | wc -l
来源：http://yup.jqgfzy.top

[R39] 重定向标准输出与错误
来源：http://vua.fengsongda.top

cmd > out.log 2>&1
来源：http://fah.snrcjt.cn

[R40] 追加写日志
来源：http://bty.fanxiaobao.xyz

echo "log" >> out.log
来源：http://moh.aibaodan.cn

[R41] 丢弃输出
来源：http://caw.kuanghao11.cn

cmd >/dev/null 2>&1
来源：http://lzb.iojbl.cn

[R42] 输入重定向
来源：http://yzj.yanxiufei.cn

wc -l < a.txt
来源：http://bpn.xziqi.cn

[R43] 按名字查找文件
来源：http://kfs.havefunace.top

find . -name "*.log" -type f
来源：http://svo.jyoumei.cn

[R44] 按修改时间查找
来源：http://lcl.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://hhg.chenzaomai.com

[R45] 批量删除
来源：http://ihu.0kj1m.cn

find . -name "*.tmp" -delete
来源：http://inq.fktsv.cn

[R46] 递归替换文件内容
来源：http://pbs.zhongyouzk.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ptg.cucudq.cn

[R47] sed 单行替换
来源：http://rfd.fanxiaobao.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://alo.sweek.top

[R48] awk 取指定列
来源：http://bxx.shanyushiyangkeji.top

awk '{print $1, $3}' a.txt
来源：http://kwj.smart0.xyz

[R49] awk 带条件
来源：http://wyd.yongpay.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pac.cheryme.top

[R50] awk 求和
来源：http://odz.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://ekh.jiagoushi.top

[R51] 排序去重取前几
来源：http://vam.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xbw.yj20258.top

[R52] 统计行数
来源：http://peb.ppjwa.cn

wc -l a.txt
来源：http://npb.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://ppk.bjfxy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bgn.shuidangran.top

[R54] 比较两个文件
来源：http://ldx.epnwcf.com

diff a.txt b.txt
来源：http://cka.sysykeji.top

[R55] 压缩与解压
来源：http://qvk.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://olg.yonumen.top

[R56] 远程拷贝
来源：http://crh.daria6918.cn

scp file user@host:/path/
来源：http://agf.cucudq.cn

[R57] 远程执行命令
来源：http://igp.jinqigfzy.top

ssh user@host 'uptime'
来源：http://hmv.yuxming.cn

[R58] 下载文件
来源：http://wko.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lao.meibo888.top

[R59] 发 POST JSON
来源：http://vui.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fje.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://wkf.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tiz.quarkkingdee.top

[R61] 磁盘占用
来源：http://vud.jqgfzy.top

df -h;  du -sh *
来源：http://rgo.smart0.xyz

[R62] 找最占空间的文件
来源：http://glm.wangdashe.top

du -ah . | sort -rh | head -10
来源：http://xms.chenjidiqi.icu

[R63] 内存与进程
来源：http://vmu.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://zrv.aibaodan.cn

[R64] 结束进程
来源：http://hfr.yanxiufei.cn

kill -9 $(pgrep -f app.py)
来源：http://tvy.yongpay.top

[R65] 查看端口占用
来源：http://bdq.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ixl.tian-w.cn

[R66] 定时任务
来源：http://tpf.vqdsnc.cn

crontab -e;  crontab -l
来源：http://lqh.ydzc1.top

[R67] 生成随机十六进制串
来源：http://bsu.fengsongda.top

openssl rand -hex 16
来源：http://wsy.cashguo.top

[R68] 计算文件校验值
来源：http://jsq.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rco.sufxvd.cn

[R69] 生成随机密码
来源：http://jcj.guowangkeji.top

head -c 16 /dev/urandom | base64
来源：http://zyr.jqgufenzy.top

[R70] 时间戳与互转
来源：http://srs.ywan-chungtsiang.top

date +%s;  date -d @1700000000
来源：http://bwp.wangdashe.top

[R71] 日期格式化
来源：http://qpb.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://suw.ywan-chungtsiang.top

[R72] 等待端口就绪
来源：http://klg.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://rgd.hesvh.cn

[R73] 分割大日志
来源：http://ons.fzhhl.top

split -l 1000 big.log part_
来源：http://xnc.chenzaomai.com

[R74] 批量重命名
来源：http://ujz.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vsh.pycfn.com

[R75] 导出环境变量
来源：http://nzc.sysykeji.top

export PATH="$HOME/bin:$PATH"
来源：http://vgv.yongpay.top

[R76] 使用临时文件
来源：http://phr.uphjek.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://okt.nanxuanxn.top

[R77] 读取用户输入
来源：http://xfn.dashuyun.cn

read -rp "请输入: " ans
来源：http://dsi.zycfv.cn

[R78] 交互式菜单
来源：http://kad.yvedp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ivn.meibo888.top

[R79] 解析命令行选项
来源：http://crb.yongpay.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://awy.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://thm.hywenlv.cn

time ./run.sh
来源：http://iae.andypj.xyz

================================================================================
来源：http://inf.yonumen.top

S. C / C++ 专题
来源：http://vet.fktsv.cn

================================================================================
来源：http://tfz.ppjwa.cn

[S01] C：Hello World
来源：http://dpx.bjfxy.top

#include <stdio.h>
来源：http://qba.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eqn.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://jje.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://kzn.zhijiandao.cn

[S03] C：读入整数
来源：http://zno.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://eeb.haohaochexian.top

[S04] C：字符串复制
来源：http://jjo.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://qtp.bjfxy.top

[S05] C：字符串长度
来源：http://hqe.hywenlv.cn

strlen(s)
来源：http://oie.vehdjk.com

[S06] C：字符串比较
来源：http://wso.guannengcc.top

strcmp(a, b) == 0
来源：http://min.yuanzhike.top

[S07] C：数组遍历求和
来源：http://oty.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kyw.316326.xyz

[S08] C：动态内存分配与释放
来源：http://mpj.fehbvm.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ahw.zycfv.cn

[S09] C：结构体定义与初始化
来源：http://ewf.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://snq.fzhhl.top

[S10] C：指针与解引用
来源：http://zmx.hesvh.cn

int *p = &a;  *p = 5;
来源：http://ekw.fzhhl.top

[S11] C：逐行读文件
来源：http://zdw.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://tnx.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://anu.haohaochexian.top

fclose(f);
来源：http://jnc.jlsjyb.cn

[S12] C：写文件
来源：http://lec.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rif.jqgfzy.top

[S13] C：宏定义
来源：http://tzd.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rwp.pycfn.com

[S14] C：枚举
来源：http://iyc.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://xfq.nanxinkj.top

[S15] C：类型转换
来源：http://mzq.jinyuanbaomall.cn

(double) a / b
来源：http://fiw.tarul.cn

[S16] C：位操作置位
来源：http://xkh.jinghuilouyu.cn

x |= (1 << 3);
来源：http://ace.xingfuxueyuan.xyz

[S17] C：安全拼接字符串
来源：http://iyx.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://shm.yj20258888.top

[S18] C：命令行参数
来源：http://rwm.birdmap.top

int main(int argc, char **argv)
来源：http://kci.kuanghao11.cn

[S19] C：快速排序
来源：http://ard.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://kti.bjfxy.top

[S20] C：二分查找
来源：http://fju.mhx1999.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yzh.xinyue.icu

[S21] C：字符类别判断
来源：http://xjm.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zfz.jinghuilouyu.cn

[S22] C：字符串转数字
来源：http://rjs.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://zhh.dashuyun.cn

[S23] C：随机数
来源：http://qhm.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rej.yuxming.cn

[S24] C：获取本地时间
来源：http://fwo.zhaomingkeji.xyz


<!-- 参考信息 -->