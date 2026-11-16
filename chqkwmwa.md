代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fud.zhiwuduotai.top

[Q50] 批量更新
来源：http://afd.zhoulong.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ixh.dashuyun.cn

[Q51] 用子查询更新
来源：http://zzj.52xcode.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ieo.smart0.xyz

[Q52] 删除指定行
来源：http://hcc.ybcxt.top

DELETE FROM users WHERE id = 10;
来源：http://pjv.chenjidiqi.icu

[Q53] 按条件删除
来源：http://jrn.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wye.zhixingplan.top

[Q54] 清空表
来源：http://gde.kuanghao11.cn

TRUNCATE TABLE logs;
来源：http://ydv.zhiwuduotai.top

[Q55] 排名（并列占位）
来源：http://ypg.dianchejie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zcz.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://gzx.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wpc.havefunace.top

[Q57] 行号
来源：http://ylv.wangshuangyany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cfq.zhoulong.xyz

[Q58] 累计求和
来源：http://mpo.0kj1m.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qvr.jinqigufen.top

[Q59] 分组内累计
来源：http://pvm.yj20258.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nzv.feifeiyinyue.top

[Q60] 取上一行 / 下一行
来源：http://vfc.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yfn.jinqigfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ixm.hcnkem.com

[Q61] 移动平均
来源：http://lmg.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jvo.smart0.xyz

[Q62] 分组占比
来源：http://uxw.ppjwa.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ihj.zhixingplan.top

[Q63] 开启事务
来源：http://nmo.guannengcc.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mgi.shanyushiyangtech.top

[Q64] 提交事务
来源：http://cth.yuanzhike.top

COMMIT;
来源：http://fig.iojbl.cn

[Q65] 回滚事务
来源：http://fre.yongpay.top

ROLLBACK;
来源：http://pes.hesvh.cn

[Q66] 行锁查询
来源：http://obc.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jlx.hesvh.cn

[Q67] 设置隔离级别
来源：http://ime.jinqigfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://huz.cheryme.top

[Q68] 保存点
来源：http://phz.bbcook.cn

SAVEPOINT sp1;
来源：http://hqz.tarul.cn

ROLLBACK TO sp1;
来源：http://hkl.xingfuxueyuan.xyz

[Q69] 查看执行计划
来源：http://gzb.wangshuangyany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jzx.jinqigfzy.top

[Q70] 更新统计信息
来源：http://lzl.gzhubu.top

ANALYZE TABLE users;
来源：http://vcr.316326.xyz

[Q71] 查看建表语句
来源：http://lrk.yj202588.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://usz.yonumen.top

[Q72] 查看索引
来源：http://jxq.jinghuilouyu.cn

SHOW INDEX FROM users;
来源：http://sqy.ybcxt.top

[Q73] 查看表状态
来源：http://ngf.xingfuxueyuan.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://fhi.ydzc1.top

[Q74] 强制使用索引
来源：http://vyh.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hhk.yj202588.top

[Q75] 日期格式化
来源：http://ugh.yuanzhike.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jex.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qou.bbcook.cn

[Q76] 按天统计
来源：http://dld.tanke756.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://thv.fanxiaobao.xyz

[Q77] 时间加减
来源：http://lrq.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tqj.yuxming.cn

[Q78] 当前时间
来源：http://upd.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rou.daxiang520.top

[Q79] 字符串拼接
来源：http://wkt.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pka.zhiwuduotai.top

[Q80] 字符串截取
来源：http://pli.zdqjudy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cqt.iojbl.cn

[Q81] 字符串替换
来源：http://knt.fehbvm.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fsa.epnwcf.com

[Q82] 字符长度与字节长度
来源：http://ztj.ybcxt.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ozl.hcnkem.com

[Q83] 大小写转换
来源：http://oiv.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ssi.hywenlv.cn

[Q84] 去除首尾空格
来源：http://qbq.jinqigufen.top

SELECT TRIM(name) FROM users;
来源：http://gml.birdmap.top

[Q85] 数值取整
来源：http://fmk.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xou.sufxvd.cn

[Q86] 读取 JSON 字段
来源：http://yes.gzhubu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rjc.yuxming.cn

[Q87] JSON 字段做条件
来源：http://xck.bjfxy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://itn.zdqjudy.top

[Q88] 行转列（条件聚合）
来源：http://ytc.chenjidiqi.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ixs.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ovn.daria6918.cn

[Q89] 判断表是否存在
来源：http://lgd.yfazqb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eys.guowangkeji.top

[Q90] 生成序号列
来源：http://lzl.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gvq.fengsongda.top

================================================================================
来源：http://dul.ywan-chungtsiang.top

R. Bash 专题
来源：http://tpr.bjfxy.top

================================================================================
来源：http://lqk.jqgfzy.top

[R01] shebang 与严格模式
来源：http://pwn.kuanghao11.cn

#!/usr/bin/env bash
来源：http://lbt.chenlongwang.top

set -euo pipefail
来源：http://kcx.zhengqikj.top

[R02] 变量赋值与使用
来源：http://eoo.jinqigfzy.top

name="Tom"; echo "$name"
来源：http://yiz.cashguo.top

[R03] 只读变量
来源：http://gqi.jiagoushi.top

readonly PI=3.14
来源：http://faw.tarul.cn

[R04] 位置参数
来源：http://hdt.aibaodan.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xyu.epnwcf.com

[R05] 参数默认值
来源：http://gzf.yj20258.top

name="${1:-default}"
来源：http://xuk.zhoulong.xyz

[R06] 判断命令是否存在
来源：http://fdc.wangdashe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://muw.zhongyouzk.top

[R07] if 判断文件
来源：http://yvr.shanyushiyangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jds.tian-w.cn

[R08] 数值比较
来源：http://lqv.zdqjudy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iwr.jqgfzy.top

[R09] 字符串比较
来源：http://wul.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://piw.wangdashe.top

[R10] 正则匹配
来源：http://qoq.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tbw.hcnkem.com

[R11] case 多分支
来源：http://jel.9152youxi.cn

case "$1" in
来源：http://hwz.wangdashe.top

start) echo "启动" ;;
来源：http://hzi.cdnleiting.top

stop)  echo "停止" ;;
来源：http://wul.havefunace.top

*)     echo "未知命令" ;;
来源：http://kiu.quarkkingdee.top

esac
来源：http://jnq.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://fvn.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://pnh.fktsv.cn

[R13] for 计数循环
来源：http://qwj.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://igu.sysykeji.top

[R14] C 风格 for
来源：http://qur.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nna.shzxlz.cn

[R15] while 逐行读文件
来源：http://lrv.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ctv.cucudq.cn

[R16] until 等待条件
来源：http://frd.chenlongwang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rsr.sufxvd.cn

[R17] 数组定义与取值
来源：http://jdk.shzxlz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mfq.hywenlv.cn

[R18] 遍历数组
来源：http://png.fengsongda.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nup.havefunace.top

[R19] 数组长度
来源：http://sbo.xuanzx.com

echo "${#arr[@]}"
来源：http://wsw.svipenyu.cn

[R20] 关联数组（字典）
来源：http://fnb.shanyushiyangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jmu.wangshuangyany.cn

[R21] 字符串长度
来源：http://hdu.xingfuxueyuan.xyz

echo "${#s}"
来源：http://qke.sufxvd.cn

[R22] 截取子串
来源：http://ocm.vqdsnc.cn

echo "${s:0:5}"
来源：http://yln.aibaodan.cn

[R23] 字符串替换
来源：http://whr.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xas.nanxinkj.top

[R24] 大小写转换
来源：http://ipg.daria6918.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qbv.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://avc.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xyv.jinyuanbaomall.cn

[R26] 命令替换
来源：http://fwp.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://nfz.ybcxt.top

[R27] 算术展开
来源：http://bys.yj20258888.top

echo $((1 + 2 * 3))
来源：http://jsg.sxryk.cn

[R28] 浮点运算
来源：http://qch.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://ezj.fehbvm.com

[R29] 定义函数
来源：http://qgb.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gfd.yuanzhike.top

[R30] 函数返回状态码
来源：http://yuz.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://cwl.jinqigufen.top

[R31] 局部变量
来源：http://mtr.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://iaj.xylfe.cn

[R32] 参数个数校验
来源：http://cfp.ppjwa.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://smo.yvedp.cn

[R33] 捕获错误并提示行号
来源：http://ndc.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ijr.aizwys.cn

[R34] 退出时清理
来源：http://zpt.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://jtf.redwolf501.top

[R35] 后台执行并等待
来源：http://twq.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://tyn.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://vej.wangshuangyany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eyy.hnxiangtu.top

[R37] 把输出赋给变量
来源：http://qiw.tian-w.cn

files=$(ls -1)
来源：http://jvc.fktsv.cn

[R38] 管道串联
来源：http://naz.kuanghao11.cn

cat a.txt | grep -i error | wc -l
来源：http://yqv.mhx1999.top

[R39] 重定向标准输出与错误
来源：http://hnn.iojbl.cn

cmd > out.log 2>&1
来源：http://slk.yuxming.cn

[R40] 追加写日志
来源：http://hiz.sysykeji.top

echo "log" >> out.log
来源：http://qth.jqgufenzy.top

[R41] 丢弃输出
来源：http://tni.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://thz.wangshuangyany.cn

[R42] 输入重定向
来源：http://vbc.redwolf501.top

wc -l < a.txt
来源：http://due.hfpthk.cn

[R43] 按名字查找文件
来源：http://zan.tarul.cn

find . -name "*.log" -type f
来源：http://gwj.aibaodan.cn

[R44] 按修改时间查找
来源：http://ahh.tarul.cn

find . -mtime -7 -type f
来源：http://qtw.hnqzz.top

[R45] 批量删除
来源：http://kad.yvedp.cn

find . -name "*.tmp" -delete
来源：http://uwp.yj20258888.top

[R46] 递归替换文件内容
来源：http://buk.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dtz.yuxming.cn

[R47] sed 单行替换
来源：http://get.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://ssr.yuxming.cn

[R48] awk 取指定列
来源：http://xyh.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://chu.sysykeji.top

[R49] awk 带条件
来源：http://rve.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eig.jinqigfzy.top

[R50] awk 求和
来源：http://lau.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ohr.zhixingplan.top

[R51] 排序去重取前几
来源：http://ncc.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://apc.shanyushiyangtech.top

[R52] 统计行数
来源：http://vfn.uphjek.com

wc -l a.txt
来源：http://lzj.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://lxa.fengsongda.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://agb.xylfe.cn

[R54] 比较两个文件
来源：http://zaz.quarkkingdee.top

diff a.txt b.txt
来源：http://hnh.ivvv.top

[R55] 压缩与解压
来源：http://vra.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mhp.zhengqikj.top

[R56] 远程拷贝
来源：http://crz.ctjpmb.com

scp file user@host:/path/
来源：http://dup.kuanghao11.cn

[R57] 远程执行命令
来源：http://dld.yuanzhike.top

ssh user@host 'uptime'
来源：http://khi.jinghuilouyu.cn

[R58] 下载文件
来源：http://rvn.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qbf.zhixingplan.top

[R59] 发 POST JSON
来源：http://eje.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://myh.ivvv.top

[R60] 只看 HTTP 状态码
来源：http://skm.svipenyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tey.hammf.cn

[R61] 磁盘占用
来源：http://ags.havefunace.top

df -h;  du -sh *
来源：http://mqg.0kj1m.cn

[R62] 找最占空间的文件
来源：http://dqt.xuanzx.com

du -ah . | sort -rh | head -10
来源：http://lyr.nanxuanxn.top

[R63] 内存与进程
来源：http://bda.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://ieh.yanxiufei.cn

[R64] 结束进程
来源：http://nvu.sysykeji.top

kill -9 $(pgrep -f app.py)
来源：http://xql.xuanzx.com

[R65] 查看端口占用
来源：http://rxi.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wui.zhiwuduotai.top

[R66] 定时任务
来源：http://ewt.zhijiandao.cn

crontab -e;  crontab -l
来源：http://mcp.ivvv.top

[R67] 生成随机十六进制串
来源：http://ycs.jlsjyb.cn

openssl rand -hex 16
来源：http://akt.tianlin.xyz

[R68] 计算文件校验值
来源：http://lgm.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://may.yfazqb.com

[R69] 生成随机密码
来源：http://wua.snrcjt.cn

head -c 16 /dev/urandom | base64
来源：http://emh.svipenyu.cn

[R70] 时间戳与互转
来源：http://avj.bjfxy.top

date +%s;  date -d @1700000000
来源：http://dvg.ydzc1.top

[R71] 日期格式化
来源：http://xfo.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rib.xingfuxueyuan.xyz

[R72] 等待端口就绪
来源：http://fao.shanyushiyangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nta.bjfxy.top

[R73] 分割大日志
来源：http://ktu.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://glr.jianghu66.top

[R74] 批量重命名
来源：http://mia.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dje.sysykeji.top

[R75] 导出环境变量
来源：http://ady.chenzaomai.com

export PATH="$HOME/bin:$PATH"
来源：http://diz.yanxiufei.cn

[R76] 使用临时文件
来源：http://sax.nanxuanxn.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tei.bbcook.cn

[R77] 读取用户输入
来源：http://xtk.vehdjk.com

read -rp "请输入: " ans
来源：http://upz.aizwys.cn

[R78] 交互式菜单
来源：http://oby.gaohongyu789.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vqq.cheryme.top

[R79] 解析命令行选项
来源：http://shr.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://osv.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://qeh.guowangkeji.top

time ./run.sh
来源：http://ftw.yangfankeji.com

================================================================================
来源：http://kkz.shangyingyoupin.top

S. C / C++ 专题
来源：http://rhz.jinyuanbaomall.cn

================================================================================
来源：http://nxe.hywenlv.cn

[S01] C：Hello World
来源：http://rye.guowangkeji.top

#include <stdio.h>
来源：http://qkd.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vvy.yj202588.top

[S02] C：变量与格式化输出
来源：http://jof.kuanghao11.cn

int a = 10; printf("%d\n", a);
来源：http://gct.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://cfp.haohaochexian.top

int x; scanf("%d", &x);
来源：http://jqz.yueranfly.top

[S04] C：字符串复制
来源：http://bwb.pengpengdd.cyou

char dst[32]; strcpy(dst, "hi");
来源：http://ydj.tianlin.xyz

[S05] C：字符串长度
来源：http://uxl.jinqigufen.top

strlen(s)
来源：http://clt.chenlongwang.top

[S06] C：字符串比较
来源：http://oot.52xcode.cn

strcmp(a, b) == 0
来源：http://glm.chenlongwang.top

[S07] C：数组遍历求和
来源：http://njw.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://agk.cashguo.top

[S08] C：动态内存分配与释放
来源：http://mkl.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yhr.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://ltx.zdbjq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qab.nanxuanxn.top

[S10] C：指针与解引用
来源：http://zna.svipenyu.cn

int *p = &a;  *p = 5;
来源：http://ejg.fzhhl.top

[S11] C：逐行读文件
来源：http://hwy.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://xgp.gogol.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cac.jinqigufen.top

fclose(f);
来源：http://xkw.shuidangran.top

[S12] C：写文件
来源：http://jff.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hfp.yongpay.top

[S13] C：宏定义
来源：http://zqq.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lyz.feifeiyinyue.top

[S14] C：枚举
来源：http://omh.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://acv.52xcode.cn

[S15] C：类型转换
来源：http://dbk.shuidangran.top

(double) a / b
来源：http://puh.ydjk.org.cn

[S16] C：位操作置位
来源：http://phs.chenjidiqi.icu

x |= (1 << 3);
来源：http://ush.nwbrower.top

[S17] C：安全拼接字符串
来源：http://zal.feifeiyinyue.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jtu.guowangkeji.top

[S18] C：命令行参数
来源：http://hfi.yueranfly.top

int main(int argc, char **argv)
来源：http://awr.dianchejie.cn

[S19] C：快速排序
来源：http://epw.nanxinkj.top

qsort(a, n, sizeof(int), cmp);
来源：http://xzx.xinyue.icu

[S20] C：二分查找
来源：http://nug.yangfankeji.com


<!-- 参考信息 -->